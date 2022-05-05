<script setup>
    import { onMounted } from 'vue'

    onMounted(() => {
        const section = document.querySelector("section.work");
        const sectionRelative = section.getBoundingClientRect();
        // const sectionPosition = (sectionRelative.top + window.scrollY);
        const content = document.querySelector("div.shots");
        // console.log("Section position: " + sectionPosition);
        // console.log("Content width: " + content.scrollWidth);

        
        if (sectionRelative.bottom > 0) {
            let newPos = "-" + content.scrollWidth + "px";
            console.log("Loaded underneath. Position: " + newPos);
            content.style.left = newPos;
        };

        document.addEventListener("scroll", event => {
            let whileSticky = section.getBoundingClientRect();
            if (whileSticky.top == 0) {
                let newPos = window.scrollY + "px";
                console.log(newPos);
                content.style.left = newPos;
            };
        });
    })
</script>

<template>
    <section class="inner grid work">
        <h2>Work</h2>
        <p>I am a multi-skilled designer with a focus on interface design, a passion for typography and design systems, an eye for detail, a strong technical leaning and an approach steeped in user-centred design.</p>
        <div class="container">
            <div class="shots">
                <img src="../assets/work-absurd-1.jpg" alt="" width="400" />
                <img src="../assets/work-prosperex-1.jpg" alt="" width="400" />
                <img src="../assets/work-seesaw-2.jpg" alt="" width="400" />
                <img src="../assets/work-prosperex-1.jpg" alt="" width="400" />
                <img src="../assets/work-absurd-1.jpg" alt="" width="400" />
                <img src="../assets/work-seesaw-2.jpg" alt="" width="400" />
                <img src="../assets/work-prosperex-1.jpg" alt="" width="400" />
                <img src="../assets/work-absurd-1.jpg" alt="" width="400" />
            </div>
        </div>
    </section>
</template>

<style scoped>
    section {
        grid-template-rows: 3;
        margin-bottom: 10rem;
    }
    h2 {
        grid-row-start: 1;
        grid-column: 1 / 5;
        padding-top: 4rem;
        margin-bottom: 2rem;
    }
    p {
        grid-row-start: 2;
        grid-column: 1 / 5;
        margin-bottom: 4rem;
    }
    .container {
        grid-row-start: 3;
        grid-column: 1 / 5;
        margin: 0 -4rem 0 -4rem;
    }
    .shots {
        display: flex;
        flex-wrap: wrap;
    }
    .shots img {
        width: 50%;
    }
    .shots img:nth-child(1) {
        order: -3;
    }
    .shots img:nth-child(2) {
        order: -1;
        width: 100%;
    }
    .shots img:nth-child(3) {
        order: -2;
    }

    @media screen and (min-width: 600px) {
        .shots img {
            width: 33.333%;
        }
        .shots img:nth-child(2) {
            width: 33.333%;
        }
    }

    @media screen and (min-width: 800px) {
        section {
            position: sticky;
            top: 0;
        }
        h2 {
            grid-column: 3 / 9;
            margin-bottom: 3rem;
        }
        p {
            grid-column: 3 / 9;
            margin-bottom: 8rem;
        }
        .container {
            grid-column: full;
            overflow-x: hidden;
            margin: unset;
        }
        .shots {
            align-items: start;
            flex-wrap: nowrap;
            aspect-ratio: 1 / 1;
        }
        .shots img {
            width: 30rem;
        }
        .shots img:nth-child(1) {
            order: -3;
        }
        .shots img:nth-child(2) {
            order: -2;
            width: 40rem;
        }
        .shots img:nth-child(3) {
            order: -1;
        }
    }
    @media screen and (min-width: 1200px) {
        section {
            margin-bottom: 70rem;
        }
        h2 {
            padding-top: 5rem;
        }
    }
    @media screen and (min-width: 1400px) {
        h2 {
            grid-column: 5 / 11;
        }
        p {
            grid-column: 5 / 11;
        }
        .shots img {
            width: 40rem;
        }
        .shots img:nth-child(2) {
            width: 50rem;
        }
    }
</style>