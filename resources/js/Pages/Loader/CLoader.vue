<template>
    <a
        href="/Landing"
        class="h-screen w-full overflow-hidden flex flex-nowrap text-center"
        id="slider"
    >
        <div
            class="bg-green-100 text-zinc-900 flex-none w-full flex flex-col items-center justify-center"
        >
            <div class="d-block">
                <img src="/images/fer.crochets.png" alt="" />
            </div>

            <p
                class="lg:block hidden text-lg text-emerald-600 animate-bounce mb-12"
            >
                Presiona la pantalla para continuar
            </p>

            <p class="lg:hidden text-base text-emerald-600 animate-bounce mb-8">
                Presiona la pantalla para continuar
            </p>

            <div class="full-screen lg:block hidden" id="myProgress">
                <div id="myBar"></div>
            </div>

            <div class="phone-screen lg:hidden" id="myProgress">
                <div id="myBar"></div>
            </div>
        </div>
    </a>
</template>
<style>
.full-screen {
    width: 100%;
    max-width: 600px;
    background: #f4f4f4;
    box-shadow: inset -1px 1px 2px rgba(200, 200, 200, 0.2),
        inset 1px -1px 2px rgba(200, 200, 200, 0.2),
        inset -1px -1px 2px rgba(255, 255, 255, 0.9),
        inset 1px 1px 3px rgba(200, 200, 200, 0.9);
    border-radius: 28px;
    overflow: hidden;
}

.phone-screen {
    width: 100%;
    max-width: 300px;
    background: #f4f4f4;
    box-shadow: inset -1px 1px 2px rgba(200, 200, 200, 0.2),
        inset 1px -1px 2px rgba(200, 200, 200, 0.2),
        inset -1px -1px 2px rgba(255, 255, 255, 0.9),
        inset 1px 1px 3px rgba(200, 200, 200, 0.9);
    border-radius: 28px;
    overflow: hidden;
}

#myBar {
    width: 10%;
    height: 30px;
    background: #a9dfbf;
    border-radius: 28px;
    text-align: center;
    line-height: 30px;
    color: white;
    transition: 0.5s;
    animation: loading82341 10s ease infinite;
}

@keyframes loading82341 {
    0% {
        width: 0%;
    }

    10% {
        width: 10%;
    }

    50% {
        width: 40%;
    }

    60% {
        width: 60%;
    }

    100% {
        width: 100%;
    }
}
.text-lg {
    font-family: "Poppins", sans-serif;
}
</style>
