<script>
    import img from "$lib/assets/loginImg.png";
</script>

<div class="flex w-screen h-screen linear-bg">
    <nav class="text-white flex px-10 py-5 gap-3 justify-between items-center absolute mt-6 left-1/2 -translate-x-1/2 w-4/5 rounded-3xl glass">
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

    <div class="w-3/5 h-full">
        <img class="h-full object-cover" src={img} alt="">
    </div>

    <div class="flex-1 h-full">

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
</style>