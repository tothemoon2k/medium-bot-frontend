<script>
    import img from "$lib/assets/loginImg.png";
    import { Input } from "$lib/components/shadcn/ui/input/index";
</script>

<div class="flex w-screen h-screen linear-bg">
    <nav class="text-white flex px-10 py-5 gap-3 justify-between items-center absolute mt-6 left-1/2 -translate-x-1/2 w-4/5 rounded-3xl glass z-10">
        <h2 class="text-2xl font-thin">The Medium Bot</h2>
        <ul class="hidden lg:flex gap-10 text-sm">
            <li class="flex gap-2 items-center">
                <img class="h-4" src="https://img.icons8.com/ios-filled/48/ffffff/dashboard.png" alt="Dashboard Icon">
                <a href="#">DASHBOARD</a>
            </li>
            <li class="flex gap-2 items-center">
                <img class="h-4" src="https://img.icons8.com/material-rounded/48/ffffff/head-profile.png" alt="Profile Icon">
                <a href="#">PROFILE</a>
            </li>
            <li class="flex gap-2 items-center">
                <img class="h-5" src="https://img.icons8.com/material-rounded/100/ffffff/name.png" alt="Sign Up Icon">
                <a href="#">SIGN UP</a>
            </li>
            <li class="flex gap-2 items-center">
                <img class="h-5" src="https://img.icons8.com/ios-glyphs/48/ffffff/password1.png" alt="Sign In Icon">
                <a href="#">SIGN IN</a>
            </li>
        </ul>
        
        <button class="hidden lg:block py-3 px-12 rounded-xl text-sm bg-blue-600">Free Download</button>

        <button class="block lg:hidden h-7">
            <img class="h-full" src="https://img.icons8.com/ios-filled/200/ffffff/menu--v6.png" alt="">
        </button>
    </nav>

    <div class="hidden lg:block lg:w-1/2 xl:w-3/5 h-full relative">
        <img class="h-full object-cover" src={img} alt="">
        <div class="w-5/6 flex flex-col gap-2 text-center text-white absolute top-1/2 -translate-y-1/2 left-1/2 -translate-x-1/2">
            <h3 class="font-thin text-2xl">Fully Automated Money Printer:</h3>
            <h2 class="tracking-[0.4rem] font-medium text-4xl">THE MEDIUM BOT DASHBOARD</h2>
        </div>
    </div>

    <div class="relative h-full flex grow flex-col justify-center items-center">
        <div class="h-fit w-3/4 flex flex-col items-center pt-8">
            <div class="text-white w-full">
                <h1 class="text-4xl">Nice to see you!</h1>
                <p class="text-gray-400">Enter your email and password to sign in</p>
            </div>

            <div class="mt-11 flex flex-col gap-7 w-full">
                <label class="flex-col text-white text-sm" for="email">Email
                    <input class="mt-2 block py-4 px-4 text-white rounded-xl w-5/6 bg-transparent border-2 border-gray-600" type="text" name="email" id="email" placeholder="lild@gmail.com">
                </label>

                <label class="flex-col text-white text-sm" for="password">Password
                    <input class="mt-2 block py-4 px-4 text-white rounded-xl w-5/6 bg-transparent border-2 border-gray-600" type="password" name="password" id="password" placeholder="Your password">
                </label>
            </div>

            <div class="mt-6 w-full flex text-white gap-3 items-center">
                <label class="switch">
                    <input type="checkbox">
                    <span class="slider"></span>
                  </label>
                <p class="text-sm">Remember Me</p>
            </div>


        <button type="button" class="mt-10 self-start w-5/6 flex justify-center text-white bg-[#4285F4] hover:bg-[#4285F4]/90 focus:ring-4 focus:ring-[#4285F4]/50 font-medium rounded-lg text-sm py-3 items-center dark:focus:ring-[#4285F4]/55">
            <svg class="mr-2 -ml-1 w-4 h-4" aria-hidden="true" focusable="false" data-prefix="fab" data-icon="google" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 488 512"><path fill="currentColor" d="M488 261.8C488 403.3 391.1 504 248 504 110.8 504 0 393.2 0 256S110.8 8 248 8c66.8 0 123 24.5 166.3 64.9l-67.5 64.9C258.5 52.6 94.3 116.6 94.3 256c0 86.5 69.1 156.6 153.7 156.6 98.2 0 135-70.4 140.8-106.9H248v-85.3h236.1c2.3 12.7 3.9 24.9 3.9 41.4z"></path></svg>
            Sign in with Google
        </button>

        <button type="button" class="mt-4 self-start w-5/6 flex justify-center text-white bg-[#24292F] hover:bg-[#24292F] focus:ring-4 focus:ring-[#4285F4]/50 font-medium rounded-lg text-sm py-3 items-center dark:focus:ring-[#4285F4]/55">
            <svg class="mr-2 -ml-1 w-4 h-4" aria-hidden="true" focusable="false" data-prefix="fab" data-icon="github" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 496 512"><path fill="currentColor" d="M165.9 397.4c0 2-2.3 3.6-5.2 3.6-3.3 .3-5.6-1.3-5.6-3.6 0-2 2.3-3.6 5.2-3.6 3-.3 5.6 1.3 5.6 3.6zm-31.1-4.5c-.7 2 1.3 4.3 4.3 4.9 2.6 1 5.6 0 6.2-2s-1.3-4.3-4.3-5.2c-2.6-.7-5.5 .3-6.2 2.3zm44.2-1.7c-2.9 .7-4.9 2.6-4.6 4.9 .3 2 2.9 3.3 5.9 2.6 2.9-.7 4.9-2.6 4.6-4.6-.3-1.9-3-3.2-5.9-2.9zM244.8 8C106.1 8 0 113.3 0 252c0 110.9 69.8 205.8 169.5 239.2 12.8 2.3 17.3-5.6 17.3-12.1 0-6.2-.3-40.4-.3-61.4 0 0-70 15-84.7-29.8 0 0-11.4-29.1-27.8-36.6 0 0-22.9-15.7 1.6-15.4 0 0 24.9 2 38.6 25.8 21.9 38.6 58.6 27.5 72.9 20.9 2.3-16 8.8-27.1 16-33.7-55.9-6.2-112.3-14.3-112.3-110.5 0-27.5 7.6-41.3 23.6-58.9-2.6-6.5-11.1-33.3 2.6-67.9 20.9-6.5 69 27 69 27 20-5.6 41.5-8.5 62.8-8.5s42.8 2.9 62.8 8.5c0 0 48.1-33.6 69-27 13.7 34.7 5.2 61.4 2.6 67.9 16 17.7 25.8 31.5 25.8 58.9 0 96.5-58.9 104.2-114.8 110.5 9.2 7.9 17 22.9 17 46.4 0 33.7-.3 75.4-.3 83.6 0 6.5 4.6 14.4 17.3 12.1C428.2 457.8 496 362.9 496 252 496 113.3 383.5 8 244.8 8zM97.2 352.9c-1.3 1-1 3.3 .7 5.2 1.6 1.6 3.9 2.3 5.2 1 1.3-1 1-3.3-.7-5.2-1.6-1.6-3.9-2.3-5.2-1zm-10.8-8.1c-.7 1.3 .3 2.9 2.3 3.9 1.6 1 3.6 .7 4.3-.7 .7-1.3-.3-2.9-2.3-3.9-2-.6-3.6-.3-4.3 .7zm32.4 35.6c-1.6 1.3-1 4.3 1.3 6.2 2.3 2.3 5.2 2.6 6.5 1 1.3-1.3 .7-4.3-1.3-6.2-2.2-2.3-5.2-2.6-6.5-1zm-11.4-14.7c-1.6 1-1.6 3.6 0 5.9 1.6 2.3 4.3 3.3 5.6 2.3 1.6-1.3 1.6-3.9 0-6.2-1.4-2.3-4-3.3-5.6-2z"></path></svg>
            Sign in with GitHub
        </button>

            <div class="mt-16 w-full">
                <button class="w-5/6 py-4 px-12 rounded-xl font-medium text-xs bg-blue-600 hover:bg-blue-700 text-white transition-all">SIGN IN</button>
                <p class="mt-7 w-5/6 text-center text-gray-300 text-sm">Don't have an account? 
                    <a class="text-white font-medium" href="/register">Sign Up</a>
                </p>
            </div> 
        </div>

        <ul class="absolute bottom-0 w-1/2 mx-auto text-white flex gap-8 text-sm">
            <li>Regulatory</li>
            <li>Regulatory</li>
            <li>Regulatory</li>
        </ul>
    </div>
</div>

<style>
    .linear-bg{
        background: linear-gradient(#0F123B, #090D2E, #020515);
    }

    .glass{
        background: rgba(113, 113, 113, 0.2);
        box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
        backdrop-filter: blur(5px);
        -webkit-backdrop-filter: blur(10px);
        border: 2px solid rgba(255, 255, 255, 0.2);
        -webkit-background-clip: padding-box;
        background-clip: padding-box;
    }

    /* The switch - the box around the slider */
.switch {
  /* Variables */
 --switch_width: 2em;
 --switch_height: 1em;
 --thumb_color: #e8e8e8;
 --track_color: #e8e8e8;
 --track_active_color: #888;
 --outline_color: #000;
 font-size: 17px;
 position: relative;
 display: inline-block;
 width: var(--switch_width);
 height: var(--switch_height);
}

/* Hide default HTML checkbox */
.switch input {
 opacity: 0;
 width: 0;
 height: 0;
}

/* The slider */
.slider {
 box-sizing: border-box;
 border: 2px solid var(--outline_color);
 position: absolute;
 cursor: pointer;
 top: 0;
 left: 0;
 right: 0;
 bottom: 0;
 background-color: var(--track_color);
 transition: .15s;
 border-radius: var(--switch_height);
}

.slider:before {
 box-sizing: border-box;
 position: absolute;
 content: "";
 height: var(--switch_height);
 width: var(--switch_height);
 border: 2px solid var(--outline_color);
 border-radius: 100%;
 left: -2px;
 bottom: -2px;
 background-color: var(--thumb_color);
 transform: translateY(-0.2em);
 box-shadow: 0 0.2em 0 var(--outline_color);
 transition: .15s;
}

input:checked + .slider {
 background-color: var(--track_active_color);
}

input:focus-visible + .slider {
 box-shadow: 0 0 0 2px var(--track_active_color);
}

/* Raise thumb when hovered */
input:hover + .slider:before {
 transform: translateY(-0.3em);
 box-shadow: 0 0.3em 0 var(--outline_color);
}

input:checked + .slider:before {
 transform: translateX(calc(var(--switch_width) - var(--switch_height))) translateY(-0.2em);
}

/* Raise thumb when hovered & checked */
input:hover:checked + .slider:before {
 transform: translateX(calc(var(--switch_width) - var(--switch_height))) translateY(-0.3em);
 box-shadow: 0 0.3em 0 var(--outline_color);
}
</style>