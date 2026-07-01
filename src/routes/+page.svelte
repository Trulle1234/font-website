<script lang="ts">
    const images = import.meta.glob("/src/lib/src_imgs/*", { eager: true, query: "?url", import: "default" });
    const srcImgs: string[] = Object.values(images) as string[];
</script>

<h1>How I made [Font name]</h1>
<p class="page-link"><a href="/font">Get the font</a> <a href="#src-imgs">See source images</a></p>


<div class="main-container">
    <div class="main-content">
        <h2>Why?</h2>
        <p>Hack Club announced the YSWS <a href="https://typeface.hackclub.com/">Typeface</a> 
            and I got the idea to take photos on my trip to Thailand and make a font by using 
            a bunch of diffrent letters from diffrent stuff.</p>

        <hr>

        <h2>How?</h2>
        <p>
            I took photos on my way to and in Thailand. 
            Then I cut them out, made them B&W and added them to a 
            <a href="https://www.calligraphr.com/">Calligraphr</a> template in Affinity.
        </p>

        <strong>That process looked something like this:</strong>
            <ol>
                <li>
                    <p>Take a photo.</p>
                    <img src="/font_src_images/1.jpg" alt="1" class="how-img">
                </li>
                <li>
                    <p>Cut it out.</p>
                    <img src="/how_images/step2.png" alt="1" class="how-img">
                </li>
                <li>
                    <p>Apply ajustment layers to make it all black.</p>
                    <img src="/how_images/step3.png" alt="1" class="how-img">
                </li>
                <li>
                    <p>Add to corresponding spot in Calligraphr template.</p>
                    <img src="/how_images/step4.png" alt="1" class="how-img">
                </li>
                <li>
                    <em>When that has been done for all charachters. Upload to Calligraphr.</em>
                </li>
            </ol>

        <hr>

        <h2 id="src-imgs">Source images <em>(Unorderd)</em></h2>
        
        <div class="src-imgs-container">
            {#each srcImgs as img}
                <img src={img} alt="1" class="src-img">
            {/each}
        </div>

    </div>
</div>