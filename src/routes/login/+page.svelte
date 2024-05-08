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

    <div class="flex-1 h-full relative flex flex-col justify-center items-center">
        <div class="h-fit w-3/4">
            <div class="text-white">
                <h1 class="text-4xl">Nice to see you!</h1>
                <p class="text-gray-400">Enter your email and password to sign in</p>
            </div>

            <div class="mt-11 flex flex-col gap-7">
                <label class="flex-col text-white text-sm" for="email">Email
                    <input class="mt-2 block py-4 px-4 text-white rounded-xl w-5/6 bg-transparent border-2 border-[#351b94]" type="text" name="email" id="email" placeholder="lild@gmail.com">
                </label>

                <label class="flex-col text-white text-sm" for="password">Password
                    <input class="mt-2 block py-4 px-4 text-white rounded-xl w-5/6 bg-transparent border-2 border-[#351b94]" type="password" name="password" id="password" placeholder="Your password">
                </label>
            </div>

            <div class="mt-6 flex text-white gap-3 items-center">
                <label class="switch">
                    <input type="checkbox">
                    <span class="slider"></span>
                  </label>
                <p class="text-sm">Remember Me</p>
            </div>

            <button class="mt-16 w-5/6 py-4 px-12 rounded-xl font-medium text-xs bg-blue-600 hover:bg-blue-700 text-white transition-all">SIGN IN</button>
        </div>

        <ul class="absolute bottom-0 left-1/2 -translate-x-1/2 text-white flex gap-8 self-end text-sm">
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