<script setup lang="ts">
import { ref } from "vue";

const r = ref(180);

setInterval(() => (r.value += -360 + Math.random() * (360 * 2)), 333);
</script>

<template>
    <div class="greeting">
        Yo.<br />
        <span class="smiley" :style="{ transform: 'rotate(' + r + 'deg)' }">🤪</span>
    </div>
    <p>Stuff i made (and didn't abandon entirely):</p>
    <ul>
        <li>
            Web platform
            <ul>
                <li><a href="https://and3k5.github.io/breathe">Breathing excercise app</a></li>
                <li><a href="https://and3k5.github.io/tetris">A simple tetris clone</a></li>
                <li>
                    <a href="https://and3k5.github.io/DataURL">A DataURL creator (no upload)</a>
                </li>
                <li>
                    <a href="https://and3k5.github.io/estimate-calc"
                        >A estimate/timebased calculator</a
                    >
                </li>
                <li>
                    <a href="https://and3k5.github.io/simple-letter-game"
                        >A game to learn the alphabet/letters</a
                    >
                </li>
                <li>
                    <a href="https://and3k5.github.io/ToneMatrix"> ToneMatrix clone </a>
                </li>
                <li>
                    <a href="https://and3k5.github.io/ImageTransform"
                        >A page that can rearrange pixels from one image to become another</a
                    >
                </li>
                <li>
                    <a href="https://and3k5.github.io/mandelbrot"
                        >Mandelbrot representation in the browser</a
                    >
                </li>
                <li>
                    <a href="https://and3k5.github.io/mouse-test"> Mouse click test utility </a>
                </li>
            </ul>
        </li>
        <li>
            javascript
            <ul>
                <li>
                    <a href="https://and3k5.github.io/lazy-var.js">A lazy variable initializer</a>
                </li>
            </ul>
            <ul>
                <li>
                    <a href="https://and3k5.github.io/timespan.js">A time representation library</a>
                </li>
            </ul>
        </li>
        <li>
            dotnet
            <ul>
                <li>
                    <a href="https://github.com/and3k5/AnotherCsvLib"
                        >My own CSV parser library for dotnet</a
                    >
                </li>
                <li>
                    <a href="https://github.com/and3k5/ConsoleXt"
                        >A console write extension/wrapper library for dotnet</a
                    >
                </li>
            </ul>
        </li>
        <li>
            rust
            <ul>
                <li>
                    <a href="https://github.com/and3k5/rust-process-list"
                        >A process list grouped by process name</a
                    >
                </li>
            </ul>
        </li>
        <li>
            user-scripts
            <ul>
                <li>
                    <a href="https://github.com/and3k5/auto-facebook-poke">
                        A tool to poke everybody back on facebook
                    </a>
                </li>
            </ul>
        </li>
    </ul>
</template>

<style scoped>
.smiley {
    display: inline-block;
    transition: transform 400ms linear;
}
.greeting {
    font-size: 24pt;
}
</style>
