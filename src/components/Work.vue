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
        <p>Here's a little sample of my work across UX and UI, visual and motion design.</p>
        <div class="shots-container">
            <div class="shots">
                <video autoplay loop muted playsinline alt="SeeSaw style tiles" width="400" height="300" loading="lazy">
                    <source src="../assets/work-seesaw-style-tiles.mp4" type="video/mp4">
                </video>
                <img srcset="../assets/work-seesaw-home-800.jpg 2x, ../assets/work-seesaw-home-400.jpg 1x" src="../assets/work-seesaw-home-800.jpg" alt="SeeSaw marketing home page" width="400" height="300" loading="lazy" />
                <img srcset="../assets/work-seesaw-mobile-800.jpg 2x, ../assets/work-seesaw-mobile-400.jpg 1x" src="../assets/work-seesaw-mobile-800.jpg" alt="SeeSaw dashboard mobile" width="400" height="300" loading="lazy" />
                <img srcset="../assets/work-seesaw-features-800.jpg 2x, ../assets/work-seesaw-features-400.jpg 1x" src="../assets/work-seesaw-features-800.jpg" alt="SeeSaw features component" width="400" height="300" loading="lazy" />
                <img srcset="../assets/work-absurd-home-800.jpg 2x, ../assets/work-absurd-home-400.jpg 1x" src="../assets/work-absurd-home-800.jpg" alt="Absurd home page" width="400" height="300" loading="lazy" />
                <video autoplay loop muted playsinline alt="Absurd clients tiles" width="400" height="300" loading="lazy">
                    <source src="../assets/work-absurd-clients.mp4" type="video/mp4">
                </video>
                <video autoplay loop muted playsinline alt="Absurd showreel" width="400" height="300" loading="lazy">
                    <source src="../assets/work-absurd-showreel.mp4" type="video/mp4">
                </video>
                <video autoplay loop muted playsinline alt="Ladbrokes onboarding journey proposal from showreel" width="400" height="300" loading="lazy">
                    <source src="../assets/work-ladbrokes-onboarding.mp4" type="video/mp4">
                </video>
                <video autoplay loop muted playsinline alt="CitySuites motion test" width="400" height="300" loading="lazy">
                    <source src="../assets/work-citysuites-motion-test.mp4" type="video/mp4">
                </video>
                <img srcset="../assets/work-prosper-ex-brand-800.jpg 2x, ../assets/work-prosper-ex-brand-400.jpg 1x" src="../assets/work-prosper-ex-brand-800.jpg" alt="Prosper EX brand definition" width="400" height="300" loading="lazy" />
                <img srcset="../assets/work-prosper-ex-employees-800.jpg 2x, ../assets/work-prosper-ex-employees-400.jpg 1x" src="../assets/work-prosper-ex-employees-800.jpg" alt="Prosper EX employee dashboard and home page detail" width="400" height="300" loading="lazy" />
                <img srcset="../assets/work-prosper-ex-dashboard-800.jpg 2x, ../assets/work-prosper-ex-dashboard-400.jpg 1x" src="../assets/work-prosper-ex-dashboard-800.jpg" alt="Prosper EX managers dashboard" width="400" height="300" loading="lazy" />
                <img srcset="../assets/work-ly-wireframes-1600.jpg 2x, ../assets/work-ly-wireframes-800.jpg 1x" src="../assets/work-ly-wireframes-1600.jpg" alt="Lucy & Yak UX" class="wide" width="400" height="300" loading="lazy" />
                <img srcset="../assets/work-esf-personas-800.jpg 2x, ../assets/work-esf-personas-400.jpg 1x" src="../assets/work-esf-personas-800.jpg" alt="Electrical Safety First personas" width="400" height="300" loading="lazy" />
                <video autoplay loop muted playsinline alt="Adidas creator app proposal" width="400" height="300" loading="lazy">
                    <source src="../assets/work-adidas-app.mp4" type="video/mp4">
                </video>
                <img srcset="../assets/work-astrazeneca-current-800.jpg 2x, ../assets/work-astrazeneca-current-400.jpg 1x" src="../assets/work-astrazeneca-current-800.jpg" alt="AstraZeneca current service blueprint" width="400" height="300" loading="lazy" />
                <img srcset="../assets/work-astrazeneca-persona-800.jpg 2x, ../assets/work-astrazeneca-persona-400.jpg 1x" src="../assets/work-astrazeneca-persona-800.jpg" alt="AstraZeneca oncology personas" width="400" height="300" loading="lazy" />
                <img srcset="../assets/work-astrazeneca-journey-800.jpg 2x, ../assets/work-astrazeneca-journey-400.jpg 1x" src="../assets/work-astrazeneca-journey-800.jpg" alt="AstraZeneca inhaler adherence user journeys" width="400" height="300" loading="lazy" />
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
        margin: 0 var(--gutter-neg);
    }

    .shots {
        display: flex;
        flex-wrap: wrap;
    }

    .shots img, .shots video {
        width: 50%;
        height: auto;
    }

    .shots img.wide, .shots video.wide {
        width: 100%;
        height: auto;
    }

    @media screen and (min-width: 600px) {
        .shots img, .shots video {
            width: 33.333%;
        }

        .shots img.wide, .shots video.wide {
            width: 66.666%;
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

        .shots img, .shots video {
            width: 25%;
        }

        .shots img.wide, .shots video.wide {
            width: 50%;
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