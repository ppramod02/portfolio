<script>
    import '../global.css';
    import './index.css';
    import Luckyman from "$lib/assets/Luckyman.svelte";
    import doryoku from "$lib/assets/doryoku.png";
    import victory from "$lib/assets/victory.png";
    import syncspace from "$lib/assets/syncspace.jpeg";
    import bloggit from "$lib/assets/bloggit.png";
    import firstpage from "$lib/assets/firstpage.png";
    import shopista from "$lib/assets/shopista.png";
    import managemint from "$lib/assets/managemint.png";
    import superstar from "$lib/assets/superstar.png";
    import github from "$lib/assets/github-mark.svg";
    import linkedin from "$lib/assets/linkedin.svg";
    import leetcode from "$lib/assets/leetcode.png";
    import location from "$lib/assets/location.svg";
    import message from "$lib/assets/message.svg";
    import download from "$lib/assets/download.svg";
    let cv = "https://drive.google.com/file/d/11ivzhqNSoxIPubHn3mnXzV2pdPBb0FcL/view?usp=sharing";
</script>

<div class='hero' id='home'>
    <div class='socials'>
        <ul>
            <li><a href='https://linkedin.com/in/ppramod02' target='_blank'>
                <img src={linkedin} class='scale' alt='logo' />
            </a></li>
            <li><a href='https://github.com/ppramod02' target='_blank'>
                <img src={github} alt='logo' />
            </a></li>
            <li><a href='https://leetcode.com/ppramod02' target='_blank'>
                <img src={leetcode} alt='logo' />
            </a></li>
        </ul>
    </div>
    <div>
        <p>Ahoy! I am</p>
        <h2>Pramod Pandey</h2>
        <p>and I make websites</p>
    </div>

    <Luckyman />
    
</div>

<div id='about'>
    <img src={doryoku} alt='doryoku man' />
    <div>
        <h2>Who Am I?</h2>
        <p>I am a dedicated and enthusiastic IT student with a passion for web development, artificial intelligence, data structures, algorithms, and programming at large. With a strong academic foundation and a relentless desire to learn, I am eager to contribute my skills and creativity to the dynamic world of technology.</p>
    </div>
</div>

<div id='projects'>
    <div class='heading'>
        <img src={victory} alt='victory man' />
        <div>
            <h2>What have I made?</h2>
            <p>Some websites, some physics simulations and some neural networks.</p>
        </div>
    </div>
    <div class='cards'>
        <div class='card project'>
            <img src={syncspace} alt='project-syncspace' />
            <h3>SyncScript</h3>
            <p>A real-time collaborative platform for developers</p>
            <span><a href='https://github.com/ppramod02/SyncScript' target="_blank">Github</a></span>
            <div class='tags'><span>socket</span><span>reactjs</span><span>nodejs</span><span>codemirror</span></div>
        </div>
        <div class='card project'>
            <img src={bloggit} alt='project-bloggit' />
            <h3>Bloggit</h3>
            <p>A minimal blogging platform</p>
            <div>
                <span><a href='https://justbloggit.netlify.app' target="_blank">Website |</a></span>
                <span><a href='https://github.com/ppramod02/Bloggit' target="_blank">Github</a></span>
            </div>
            <div class='tags'><span>web dev</span><span>reactjs</span><span>firebase</span></div>
        </div>
        <div class='card project'>
            <img src={firstpage} alt='project-firstPage' />
            <h3>First Page</h3>
            <p>Book Exploration Platform</p>
            <div>
                <span><a href='https://first-page-books.netlify.app' target="_blank">Website |</a></span>
                <span><a href='https://github.com/ppramod02/firstPage' target="_blank">Github</a></span>
            </div>
            <div class='tags'><span>web dev</span><span>reactjs</span><span>supabase</span></div>
        </div>
        <div class='card project'>
            <img src={shopista} alt='project-firstPage' />
            <h3>Shopista</h3>
            <p>Ecommerce platform</p>
            <div>
                <span><a href='https://shopista-profile.netlify.app' target="_blank">Website |</a></span>
                <span><a href='https://github.com/ppramod02/shopista' target="_blank">Github</a></span>
            </div>
            <div class='tags'><span>firebase</span><span>reactjs</span><span>assignment</span></div>
        </div>
        <div class='card project'>
            <img src={managemint} alt='project-firstPage' />
            <h3>ManageMint</h3>
            <p>CMS platform</p>
            <div>
                <span><a href='https://managemint.netlify.app' target="_blank">Website |</a></span>
                <span><a href='https://github.com/ppramod02/ecowiser-frontend' target="_blank">Github</a></span>
            </div>
            <div class='tags'><span>postgres</span><span>nextjs</span><span>assignment</span></div>
        </div>
        <div class='card project'>
            <h3>A basic Perceptron network</h3>
            <p>Capable of solving linearly separable problems</p>
            <span><a href='https://github.com/ppramod02/Neural-Networks/tree/main/Perceptron' target="_blank">Github</a></span>
            <div class='tags'><span>neural networks</span><span>AI-ML</span><span>mathematics</span></div>
        </div>
        <div class='card project'>
            <h3>XOR Identifier</h3>
            <p>Capable of solving non-linearly separable problems</p>
            <span><a href='https://github.com/ppramod02/Neural-Networks/tree/main/NN_XOR' target="_blank">Github</a></span>
            <div class='tags'><span>neural networks</span><span>AI-ML</span><span>mathematics</span></div>
        </div>        
        <div class='card project'>
            <h3>Inverse Fourier Drawing</h3>
            <p>Convert drawings to fourier series</p>
            <div>
                <span><a href='https://drawfourier.netlify.app/' target="_blank">Website |</a></span>
                <span><a href='https://github.com/ppramod02/2D-Simulations/tree/main/Fourier%20Transform' target="_blank">Github</a></span>
            </div>
            <div class='tags'><span>simulations</span><span>physics</span><span>mathematics</span></div>
        </div>
        <div class='card project'>
            <h3>Fourier Series Generator</h3>
            <p>Generate Fourier series of different ampl. and freqs.</p>
            <span><a href='https://github.com/ppramod02/2D-Simulations/tree/main/Fourier%20Series' target="_blank">Github</a></span>
            <div class='tags'><span>simulations</span><span>physics</span><span>mathematics</span></div>
        </div>
    </div>
</div>

<div id='skills'>
    <div class='heading'>
        <div>
            <h2>What Am I Good At?</h2>
            <p>Well, a lot of things but some of them would be...</p>
        </div>
        <img src={superstar} alt='superstar man' />
    </div>
    <div class='cards'>
        <div class="card"><p>ReactJS</p></div>
        <div class="card"><p>Data Structures & Algos</p></div>
        <div class="card"><p>2D simulations</p></div>
        <div class="card"><p>Neural Networks</p></div>
        <div class="card"><p>Node & ExpressJS</p></div>
        <div class="card"><p>MongoDB</p></div>
        <div class="card"><p>Firebase</p></div>
        <div class="card"><p>Web Development</p></div>
    </div>
</div>

<footer>
    <a href='https://linkedin.com/in/ppramod02' target='_blank'><img src={message} alt='logo' />Connect with me</a>
    <p><img src={location} alt='logo' />Bhopal MP, India</p>
    <a href={cv} download="PramodPandeyResume"><img src={download} alt='logo' />Download CV</a>
    <p>This website is made using <a style='text-decoration:underline' href='https://kit.svelte.dev/'>SvelteKit</a></p>
</footer>
