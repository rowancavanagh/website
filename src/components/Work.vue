<script setup>
    //
    // Struggling to get the position of the shots relative to the page, ignoring the sticky positioning
    //
    // import { onMounted } from 'vue'

    // onMounted(() => {
    //     const section = document.querySelector("div.shots");
    //     const sectionRelative = section.getBoundingClientRect();
    //     // const sectionPosition = (sectionRelative.top + window.scrollY);
    //     const content = document.querySelector("div.shots");
    //     // console.log("Section position: " + sectionPosition);
    //     // console.log("Content width: " + content.scrollWidth);

    //     console.log("Position top: " + sectionRelative.top + ". Position bottom: " + sectionRelative.bottom);
    //     if (sectionRelative.bottom < 0) {
    //         let newPos = "-" + content.scrollWidth + "px";
    //         console.log("Loaded underneath. New pos: " + newPos);
    //         content.style.left = newPos;
    //     };

    //     document.addEventListener("scroll", event => {
    //         let whileSticky = section.getBoundingClientRect();
    //         if (whileSticky.top == 0) {
    //             let newPos = window.scrollY + "px";
    //             console.log(newPos);
    //             content.style.left = newPos;
    //         };
    //     });
    // })
</script>

<template>
    <section class="inner grid work">
        <h2>Work</h2>
        <p>I am a multi-skilled designer with a focus on interface design, a passion for typography and design systems, an eye for detail, a strong technical leaning and an affinity for user-centred design.</p>
        <p>Here's a little sample of my work, while I get on to writing case studies!</p>
        <div class="shots-container">
            <div class="shots">
                <img src="../assets/placeholder-1.jpg" alt="" width="400" />
                <img src="../assets/placeholder-2.jpg" alt="" width="400" />
                <img src="../assets/placeholder-3.jpg" alt="" width="400" />
                <img src="../assets/placeholder-4.jpg" alt="" width="400" />
                <img src="../assets/placeholder-5.jpg" alt="" width="400" />
                <img src="../assets/placeholder-6.jpg" alt="" width="400" />
            </div>
        </div>
    </section>
</template>

<style scoped>
    section {
        margin-bottom: 10rem;
    }
    h2 {
        grid-column: 1 / 5;
        margin-bottom: 2rem;
    }
    p {
        grid-column: 1 / 5;
        margin-bottom: 2rem;
    }
    p:last-of-type {
        margin-bottom: 4rem;
    }
    .shots-container {
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
    @media screen and (max-width: 599px) {
        .shots img:nth-child(3) {
            width: 100%;
        }
    }

    @media screen and (min-width: 600px) {
        .shots img {
            width: 33.333%;
        }
    }

    @media screen and (min-width: 800px) {
        h2 {
            grid-column: 3 / 9;
            margin-bottom: 3rem;
        }
        p {
            grid-column: 3 / 9;
        }
        p:last-of-type {
            margin-bottom: 8rem;
        }
        .shots-container {
            grid-column: full;
            margin: unset;
        }
        .shots img {
            width: 25%;
        }
    }
    @media screen and (min-width: 1200px) {
        section {
            margin-bottom: 25rem;
        }
    }
    @media screen and (min-width: 1400px) {
        h2 {
            grid-column: 5 / 11;
        }
        p {
            grid-column: 5 / 11;
        }
        /* .shots img {
            width: 20%;
        } */
    }

    /* CSS for the sticky horizontal scroll shots */
    /*
    @media screen and (min-width: 800px) {
        section {
            position: sticky;
            top: 0;
        }
        .shots-container {
            grid-column: full;
            overflow-x: hidden;
            margin: unset;
            aspect-ratio: 1 / 1;
        }
        .shots {
            align-items: center;
            flex-wrap: nowrap;
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
    */
</style>