<script>
    let cursor;
    const handleMouseMove = (event) => {
        if(cursor) {
            let keyframes = { left: `${event.clientX - 20}px`, top: `${event.clientY + window.scrollY - 20}px` };
            cursor.animate(keyframes, {
                fill: 'forwards',
                duration: 600,
            });
        }
    }

</script>

<div class='cursor' bind:this={cursor}></div>

<div on:mousemove={handleMouseMove} role='region'>
    <nav>
        <ul>
            <li><a href='#home'>Home</a></li>
            <li><a href='#about'>About</a></li>
            <li><a href='#projects'>Projects</a></li>
            <li><a href='#skills'>Skills</a></li>
        </ul>
    </nav>

    <aside>
        <slot />
    </aside>
</div>

<style>
    .cursor {
        z-index: 30;
        pointer-events: none;
        position: absolute;
        height: 40px;
        width: 40px;
        border: 1px solid var(--dark);
        border-radius: 50vw;
    }
    nav {
        z-index: 25;
        position: fixed;
        bottom: 0;
        left: 50%;
        display: flex;
        justify-content: center;
        width: clamp(300px, 100vw, 700px);
        transform: translateX(-50%);
        padding: 1rem;
        background: rgb(255 255 255 / 0.2);
        backdrop-filter: blur(10px);
    }

    nav ul {
        list-style-type: none;
        display: flex;
        gap: 2.5rem;
    }

    nav ul li {
        font-size: 1.1rem;
        transition: all 200ms ease;
    }
    
    nav ul li:hover {
        font-weight: 500;
        scale: 1.15;
    }

    nav ul:has(li:hover) li:not(:hover) {
        scale: 0.8;
        opacity: 50%;
    }
</style>