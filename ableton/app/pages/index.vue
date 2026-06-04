<template>
    <div class="flex justify-center min-h-screen w-full bg-gray-200 px-20">    
        <div class="flex flex-col min-h-screen bg-white w-full mx-10">
            <Navbar />
            <main class="relative flex flex-col h-full gap-6 mb-4">
                <section class="sticky top-6 bg-transparent z-20 mt-6 px-10">
                    <div class="flex gap-6 ">
                        <button type="button" class="text-[#ff764d] font-bold">
                            About
                        </button>
                        <button type="button" class="font-bold">
                            Jobs
                        </button>
                        <button type="button" class="font-bold">
                            Apprenticeships
                        </button>
                    </div>
                </section>
                <section class="flex flex-col gap-10 justify-center items-center">
                    <div class="relative px-10">
                        <svg class="absolute top-90 left-0 z-10 w-full text-[#ff764d] text-10xl" with="430px" height="104px" viewBox="0 0 430 104"><title>Ableton</title><g fill="#FD5948"><path d="M32.6204615,65.1749841 L47.5563462,31.7794286 L62.5038077,65.1749841 L32.6204615,65.1749841 L32.6204615,65.1749841 Z M93.8623846,100.13219 C86.5871154,84.2631111 78.9777692,67.7271111 71.3717308,51.1878095 C63.7656923,34.6567619 56.1629615,18.1306667 48.8810769,2.24342857 C48.6313462,1.7944127 48.1550385,1.51873016 47.6076154,1.51873016 C47.0535769,1.51873016 46.5326154,1.80101587 46.2134231,2.27644444 L1.24534615,100.156952 C1.08823077,100.634032 1.13619231,101.121016 1.38923077,101.467683 C1.63565385,101.807746 2.05407692,101.994286 2.57007692,101.994286 L15.2071154,101.994286 C15.6916923,101.994286 16.1431923,101.688889 16.5467308,101.073143 L26.9097308,78.3235556 L68.2145385,78.3235556 L68.2806923,78.4688254 C69.7145769,81.6614603 71.2427308,84.9779048 72.7245769,88.1870476 C74.7009231,92.4791111 76.7483846,96.9147937 78.5924231,101.10946 C78.9777692,101.695492 79.4176923,101.994286 79.9155,101.994286 L92.5459231,101.994286 C93.0635769,101.994286 93.4853077,101.807746 93.7300769,101.467683 C93.9831154,101.116063 94.0310769,100.629079 93.8623846,100.13219 Z M131.990154,91.6751746 C121.000346,91.6751746 115.246615,81.7786667 115.246615,72.0043175 C115.246615,62.6525714 121.117769,52.7147937 131.990154,52.7147937 C142.230769,52.7147937 149.382,60.6468571 149.382,72.0043175 C149.382,81.7968254 144.002038,91.6751746 131.990154,91.6751746 Z M134.6975,40.3420952 C127.597538,40.3420952 121.455154,43.0840635 116.445654,48.4970159 L116.020615,48.9559365 L116.020615,2.52571429 C116.020615,2.01066667 115.349154,1.35860317 114.595,1.35860317 L103.375308,1.35860317 C102.616192,1.35860317 101.941423,2.01066667 101.941423,2.52571429 L101.941423,100.698413 C101.941423,101.428063 102.573192,101.994286 103.375308,101.994286 L114.461038,101.994286 C115.264808,101.994286 115.891615,101.428063 115.891615,100.698413 L115.891615,95.463746 L116.315,95.896254 C121.284808,101.000508 127.802615,103.924063 134.186462,103.924063 C154.034269,103.924063 163.070885,87.247746 163.070885,71.7484444 C163.070885,56.5215238 153.127962,40.3420952 134.6975,40.3420952 Z M184.660192,1.35860317 L173.574462,1.35860317 C172.815346,1.35860317 172.142231,2.01066667 172.142231,2.52571429 L172.142231,100.698413 C172.142231,101.428063 172.770692,101.994286 173.574462,101.994286 L184.660192,101.994286 C185.287,101.994286 185.958462,101.475937 185.958462,100.698413 L185.958462,2.52571429 C185.958462,2.03542857 185.305192,1.35860317 184.660192,1.35860317 Z M210.465154,65.1749841 L210.554462,64.8629841 C212.320769,58.6989206 217.836346,52.4589206 224.966077,52.4589206 C232.990538,52.4589206 237.609731,58.8673016 239.255308,64.8629841 L239.338,65.1749841 L210.465154,65.1749841 Z M224.966077,40.3420952 C206.912692,40.3420952 195.702923,52.6702222 195.702923,72.5210159 C195.702923,91.0099048 207.843808,103.924063 225.230692,103.924063 C236.9945,103.924063 246.973808,97.9250794 252.600192,87.4606984 L252.694462,87.2791111 C252.754,86.8631111 252.492692,86.4421587 251.887385,85.9617778 L242.510077,80.7106032 C241.805538,80.3078095 241.266385,80.3936508 240.761962,81.0308571 C237.024269,87.0546032 233.503231,91.6751746 225.354731,91.6751746 C216.546346,91.6751746 210.179038,85.7950476 209.515846,77.0408889 L209.494346,76.7784127 L252.041192,76.7784127 C252.730846,76.7784127 253.471769,76.4119365 253.471769,75.6063492 L253.471769,73.8102857 C253.471769,58.3704127 246.009615,40.3420952 224.966077,40.3420952 Z M297.834538,42.1398095 L284.053038,42.1398095 L284.053038,26.4539683 C284.053038,25.7325714 283.555231,25.2868571 282.7465,25.2868571 L271.665731,25.2868571 C270.954577,25.2868571 270.235154,25.6450794 270.235154,26.4539683 L270.235154,33.0208254 C270.235154,35.9790476 270.235154,42.1398095 261.997346,42.1398095 L259.677,42.1398095 C258.917885,42.1398095 258.243115,42.7951746 258.243115,43.3151746 L258.243115,53.7366349 C258.243115,54.7023492 259.339615,54.7749841 259.677,54.7749841 L270.235154,54.7749841 L270.235154,80.0651429 C270.235154,96.3188571 276.301462,103.884444 289.327154,103.884444 C293.114462,103.884444 296.132731,103.427175 298.304231,102.519238 L298.297615,102.469714 C298.816923,102.369016 299.261808,101.707048 299.261808,101.424762 L299.261808,90.4915556 C299.261808,89.8543492 298.608538,89.3161905 297.834538,89.3161905 C297.555038,89.3161905 297.062192,89.487873 296.891846,89.5572063 C295.315731,90.1828571 293.688346,90.8349206 291.351462,90.8349206 C290.818923,90.8349206 290.258269,90.8019048 289.682731,90.7325714 C283.998462,89.4697143 284.031538,82.0097778 284.053038,77.0755556 L284.053038,54.7749841 L297.834538,54.7749841 C298.168615,54.7749841 299.261808,54.7023492 299.261808,53.7366349 L299.261808,43.3151746 C299.261808,42.7951746 298.588692,42.1398095 297.834538,42.1398095 Z M337.118346,90.9092063 C327.102654,90.9092063 318.954154,82.4819048 318.954154,72.1297778 C318.954154,61.8552381 327.102654,53.4906667 337.118346,53.4906667 C347.272962,53.4906667 355.538885,61.8552381 355.538885,72.1297778 C355.538885,82.4819048 347.272962,90.9092063 337.118346,90.9092063 Z M337.118346,40.3420952 C319.112923,40.3420952 305.010577,54.3028571 305.010577,72.1297778 C305.010577,89.9583492 319.112923,103.924063 337.118346,103.924063 C355.123769,103.924063 369.227769,89.9583492 369.227769,72.1297778 C369.227769,54.3028571 355.123769,40.3420952 337.118346,40.3420952 Z M407.623462,40.3420952 C401.669615,40.3420952 395.856346,42.6697143 392.075654,46.5721905 L391.680385,46.9815873 L391.529885,43.3168254 C391.529885,42.791873 390.855115,42.1398095 390.092692,42.1398095 L379.008615,42.1398095 C378.2495,42.1398095 377.578038,42.791873 377.578038,43.3069206 L377.578038,100.698413 C377.578038,101.428063 378.2065,101.994286 379.008615,101.994286 L390.092692,101.994286 C390.898115,101.994286 391.529885,101.428063 391.529885,100.698413 L391.529885,74.4507937 C391.529885,64.7688889 391.529885,52.7180952 404.272769,52.7180952 C414.749885,52.7180952 415.603269,59.5886984 415.603269,67.8905397 L415.603269,100.698413 C415.603269,101.428063 416.231731,101.994286 417.032192,101.994286 L428.121231,101.994286 C428.888615,101.994286 429.422808,101.464381 429.422808,100.698413 L429.422808,66.4708571 C429.422808,48.399619 422.699923,40.3420952 407.623462,40.3420952 Z" id="Fill-9" sketch:type="MSShapeGroup"></path></g></svg>
                        <img class="z-0" src="https://ableton-production.imgix.net/about/header.jpg?auto=compress%2Cformat&w=1400" alt="ableton
                        " width="1400" />
                    </div>

                    <div class="flex justify-center items-center my-10">
                        <div class="flex flex-col gap-4 w-1/2">
                            <h1 class="font-semibold text-2xl">
                                We make <span class="text-[#0000FF]">Live</span>, <span class="text-[#0000FF]"> Push</span>, <span class="text-[#0000FF]">Note </span>, <span class="text-[#0000FF]"> Move</span> and <span class="text-[#0000FF]"> Link </span> — unique software and hardware for music creation and performance. With these products, our community of users creates amazing things.
                            </h1>
                            <p class="text-md">
                                Ableton was founded in 1999 and released the first version of Live in 2001. Our products are used by a community of dedicated musicians, sound designers, and artists from across the world.
                            </p>
                        </div>
                    </div>

                    <div class="relative w-full h-220 my-10">
                        <div class="absolute top-0 right-0 z-0 w-240 h-full bg-[#FBFFA8]"> </div>
                        <img class="z-20 absolute top-30 left-20 w-180 h-3/4" src="https://ableton-production.imgix.net/about/photo-1.jpg?auto=compress%2Cformat&w=800" alt="img"/>
                        <img class="z-10 absolute top-60 right-30 w-140 h-100" src="https://ableton-production.imgix.net/about/photo-2.jpg?auto=compress%2Cformat&w=800" alt="img"/>
                    </div>
                    
                    <div class="flex justify-center items-center my-10">
                        <div class="flex flex-col gap-10 w-200">
                            <div class="flex flex-col gap-4 my-10">
                                <h1 class="font-semibold text-2xl">
                                    Making music isn’t easy. It takes time, effort, and learning. But when you’re in the flow, it’s incredibly rewarding.
                                </h1>
                                <p class="text-md">
                                    We feel the same way about making Ableton products. The driving force behind Ableton is our passion for what we make, and the people we make it for.
                                </p>
                            </div>
                            <div class="flex flex-col justify-center self-center w-full gap-2">
                                <iframe height="460" src="https://www.youtube.com/embed/9SbnhgjeyXA?si=1BvUmWbDtFBWOz9y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
                                <span class="font-bold">
                                    Why Ableton - Juanpe Bolivar
                                </span>
                            </div>

                            <div class="flex flex-col gap-4 my-10">
                                <h1 class="font-semibold text-2xl">
                                    We are more than 350 people from 30 different countries divided between our headquarters in Berlin and our offices in Los Angeles and Tokyo.
                                </h1>
                                <p class="text-md">
                                    Most of us are active musicians, producers, and DJs, and many of us use Live and Push every day. We come from a wide range of cultural and professional backgrounds. Some of us have PhDs, some are self-taught, and most of us are somewhere in between. What connects us is the shared belief that each of us has the skills and knowledge to contribute to something big: helping to shape the future of music culture.
                                </p>
                            </div>
                        </div>
                    </div>
                    <div class="relative w-full h-300 my-10">
                        <div class="absolute top-0 left-0 z-0 w-240 h-full bg-[#b6ffc0]"> </div>
                        <img alt="" class="z-20 absolute top-40 left-35 w-140 h-100" src="https://ableton-production.imgix.net/about/photo-3.jpg?auto=compress%2Cformat&amp;w=180" srcset="
                            https://ableton-production.imgix.net/about/photo-3.jpg?auto=compress%2Cformat&amp;w=180 180w,
                            https://ableton-production.imgix.net/about/photo-3.jpg?auto=compress%2Cformat&amp;w=268 268w,
                            https://ableton-production.imgix.net/about/photo-3.jpg?auto=compress%2Cformat&amp;w=360 360w,
                            https://ableton-production.imgix.net/about/photo-3.jpg?auto=compress%2Cformat&amp;w=400 400w,
                            https://ableton-production.imgix.net/about/photo-3.jpg?auto=compress%2Cformat&amp;w=600 600w,
                            https://ableton-production.imgix.net/about/photo-3.jpg?auto=compress%2Cformat&amp;w=800 800w,
                            https://ableton-production.imgix.net/about/photo-3.jpg?auto=compress%2Cformat&amp;w=1200 1200w
                        " sizes="34vw">
                        <img alt="" class="z-20 absolute top-160 left-35 w-140 h-100" src="https://ableton-production.imgix.net/about/photo-4.jpg?auto=compress%2Cformat&amp;w=180" srcset="
                            https://ableton-production.imgix.net/about/photo-4.jpg?auto=compress%2Cformat&amp;w=180 180w,
                            https://ableton-production.imgix.net/about/photo-4.jpg?auto=compress%2Cformat&amp;w=268 268w,
                            https://ableton-production.imgix.net/about/photo-4.jpg?auto=compress%2Cformat&amp;w=360 360w,
                            https://ableton-production.imgix.net/about/photo-4.jpg?auto=compress%2Cformat&amp;w=400 400w,
                            https://ableton-production.imgix.net/about/photo-4.jpg?auto=compress%2Cformat&amp;w=600 600w,
                            https://ableton-production.imgix.net/about/photo-4.jpg?auto=compress%2Cformat&amp;w=800 800w,
                            https://ableton-production.imgix.net/about/photo-4.jpg?auto=compress%2Cformat&amp;w=1200 1200w
                        " sizes="34vw">
                        <img alt="" class="z-20 absolute top-60 right-30 w-160 h-160" src="https://ableton-production.imgix.net/about/photo-5.jpg?auto=compress%2Cformat&amp;w=180" srcset="
                            https://ableton-production.imgix.net/about/photo-5.jpg?auto=compress%2Cformat&amp;w=180 180w,
                            https://ableton-production.imgix.net/about/photo-5.jpg?auto=compress%2Cformat&amp;w=268 268w,
                            https://ableton-production.imgix.net/about/photo-5.jpg?auto=compress%2Cformat&amp;w=360 360w,
                            https://ableton-production.imgix.net/about/photo-5.jpg?auto=compress%2Cformat&amp;w=400 400w,
                            https://ableton-production.imgix.net/about/photo-5.jpg?auto=compress%2Cformat&amp;w=600 600w,
                            https://ableton-production.imgix.net/about/photo-5.jpg?auto=compress%2Cformat&amp;w=800 800w,
                            https://ableton-production.imgix.net/about/photo-5.jpg?auto=compress%2Cformat&amp;w=1200 1200w
                        " sizes="42vw">
                    </div>
 
                    <div class="flex justify-center items-center my-10">
                        <div class="flex flex-col gap-4 w-1/2">
                            <h1 class="font-semibold text-2xl">
                                We believe it takes focus to create truly outstanding instruments. We only work on a few products and we strive to make them great.
                            </h1>
                            <p class="text-md">
                                Rather than having a one-size-fits-all process, we try to give our people what they need to work their magic and grow. We’ve learned that achieving the best results comes from building teams that are richly diverse, and thus able to explore problems from a wider set of perspectives. We don’t always agree with each other, but opinion and debate are valued and openly encouraged.
                            </p>
                        </div>       
                    </div>

                    <div>
                        <img class="my-10" src="https://ableton-production.imgix.net/about/poster-meet-the-makers.jpg?auto=compress%2Cformat&w=1200" alt="yaur" />
                    </div>


                    <div class="flex justify-center items-center my-10">
                        <div class="flex flex-col gap-4 w-1/2">
                            <h1 class="font-semibold text-2xl">
                                We’re passionate about what we do, but we’re equally passionate about improving who we are.
                            </h1>
                            <p class="text-md">
                                We work hard to foster an environment where people can grow both personally and professionally, and we strive to create a wealth of opportunities to learn from and with each other.
                            </p>
                            <p class="text-md">
                                Alongside an internal training program, employees are actively supported in acquiring new knowledge and skills, and coached on applying these in their daily work. In addition, staff-organized development and music salons are a chance to discuss new technologies, production techniques and best practices.
                            </p>
                        </div>       
                    </div>

                    <div class="relative w-full h-240 my-10">
                        <div class="absolute w-260 left-70 z-0 bg-[#d5b3ff] h-full"></div>
                        <img alt="" class="absolute z-10 top-70 left-30 w-136 h-100" src="https://ableton-production.imgix.net/about/photo-6-a.jpg?auto=compress%2Cformat&amp;w=180" srcset="
                            https://ableton-production.imgix.net/about/photo-6-a.jpg?auto=compress%2Cformat&amp;w=180 180w,
                            https://ableton-production.imgix.net/about/photo-6-a.jpg?auto=compress%2Cformat&amp;w=268 268w,
                            https://ableton-production.imgix.net/about/photo-6-a.jpg?auto=compress%2Cformat&amp;w=360 360w,
                            https://ableton-production.imgix.net/about/photo-6-a.jpg?auto=compress%2Cformat&amp;w=400 400w,
                            https://ableton-production.imgix.net/about/photo-6-a.jpg?auto=compress%2Cformat&amp;w=600 600w,
                            https://ableton-production.imgix.net/about/photo-6-a.jpg?auto=compress%2Cformat&amp;w=800 800w,
                            https://ableton-production.imgix.net/about/photo-6-a.jpg?auto=compress%2Cformat&amp;w=1200 1200w
                        " sizes="20vw">

                       <img alt="" class="absolute top-36 right-0 w-160 h-160" src="https://ableton-production.imgix.net/about/photo-7.jpg?auto=compress%2Cformat&amp;w=180" srcset="
                            https://ableton-production.imgix.net/about/photo-7.jpg?auto=compress%2Cformat&amp;w=180 180w,
                            https://ableton-production.imgix.net/about/photo-7.jpg?auto=compress%2Cformat&amp;w=268 268w,
                            https://ableton-production.imgix.net/about/photo-7.jpg?auto=compress%2Cformat&amp;w=360 360w,
                            https://ableton-production.imgix.net/about/photo-7.jpg?auto=compress%2Cformat&amp;w=400 400w,
                            https://ableton-production.imgix.net/about/photo-7.jpg?auto=compress%2Cformat&amp;w=600 600w,
                            https://ableton-production.imgix.net/about/photo-7.jpg?auto=compress%2Cformat&amp;w=800 800w,
                            https://ableton-production.imgix.net/about/photo-7.jpg?auto=compress%2Cformat&amp;w=1200 1200w
                        " sizes="40vw"> 
                    </div>
                    <div class="flex justify-center items-center my-10">
                        <div class="flex flex-col gap-4 w-1/2">
                            <h1 class="font-semibold text-2xl">
                               We want our employees to love it here. Since we’re looking for exceptional talent from around the world, we will do everything we can to make your transition as easy as possible.
                            </h1>
                            <p class="text-md">
                                If you're joining us in Berlin, we'll help with relocation and paperwork. We’ll even provide you with free German or English lessons. Plus, working in Germany means you can expect comprehensive health insurance for you and your family, as well as generous maternity and paternity leave. Office hours are flexible, but it’s not all work; we have several company and team outings throughout the year as well as a variety of fun, informal small-group activities.
                            </p>
                        </div>       
                    </div>

                    <div class="flex justify-center h-160 items-center my-10">
                        <div class="flex w-3/4 h-full">
                            <div class="flex-1 border h-full">
                                <img alt="" class="w-full h-full" src="https://ableton-production.imgix.net/about/photo-8.jpg?auto=compress%2Cformat&amp;w=180" srcset="
                                    https://ableton-production.imgix.net/about/photo-8.jpg?auto=compress%2Cformat&amp;w=180 180w,
                                    https://ableton-production.imgix.net/about/photo-8.jpg?auto=compress%2Cformat&amp;w=268 268w,
                                    https://ableton-production.imgix.net/about/photo-8.jpg?auto=compress%2Cformat&amp;w=360 360w,
                                    https://ableton-production.imgix.net/about/photo-8.jpg?auto=compress%2Cformat&amp;w=400 400w,
                                    https://ableton-production.imgix.net/about/photo-8.jpg?auto=compress%2Cformat&amp;w=600 600w,
                                    https://ableton-production.imgix.net/about/photo-8.jpg?auto=compress%2Cformat&amp;w=800 800w,
                                    https://ableton-production.imgix.net/about/photo-8.jpg?auto=compress%2Cformat&amp;w=1200 1200w
                                " sizes="(min-width: 80em) 50vw, 84vw">
                            </div>
                            <div class="flex justify-center items-center flex-1 bg-[#b1c5ff]">
                                <div class="flex flex-col gap-6 w-1/2">
                                        <h1 class="font-semibold text-2xl tracking-wide">
                                        We’re really proud of the work we’ve done so far. But there’s so much more to come. If you’d like to be a part of it, please join us.
                                    </h1>
                                    <div class="flex text-2xl items-end cursor-pointer">
                                        <h1 class="font-semibold text-[#0000FF]">
                                            See latest jobs
                                        </h1>
                                        <ChevronRight color="#0000FF" :size="24"/>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </section>

                <footer class="flex flex-col gap-10 px-10">
                    <h1 class="font-bold text-4xl">
                        Ableton
                    </h1>
                    <div class="flex">
                        <div class="flex-1 flex gap-2 flex-col">
                            <span class="flex gap-2 items-center">
                                Register Live or Push
                                <ChevronRight :size="16"/>
                            </span>
                            <span class="flex gap-2 items-center">
                                About Ableton
                                <ChevronRight :size="16"/>
                            </span>
                            <span class="flex gap-2 items-center">
                                Jobs
                                <ChevronRight :size="16"/>
                            </span>
                            <div class="flex gap-2">
                                <Facebook />
                                <TwitterX />
                                <Youtube />
                                <Instagram />
                            </div>
                        </div>
                        <div class="flex-1 flex gap-2 flex-col">
                            <span>
                                Education
                            </span>
                            <span class="flex gap-2 items-center">
                                Offers for students and teachers
                                <ChevronRight :size="16"/>
                            </span>
                            <span class="flex gap-2 items-center">
                                Offers for institutions
                                <ChevronRight :size="16"/>
                            </span>
                            <span class="flex gap-2 items-center">
                                Push 1 trade-in initiative
                                <ChevronRight :size="16"/>
                            </span>
                        </div>
                        <div class="flex-1 flex gap-2 flex-col">
                            <span>
                                Sign up to our newsletter
                            </span>
                            <span>
                                Enter your email address to stay up to date with latest offers, tutorials, downloads and more
                            </span>
                            <div class="flex">
                                <input class="border" type="email" placeholder="Email address"/>
                                <button class="bg-[#0000FF] w-20 h-8 border text-center text-white" type="submit">
                                    Sign Up
                                </button>
                            </div>
                        </div>
                    </div>
                    <div class="flex">
                        <div class="flex-1 flex gap-2 flex-col">
                            <span class="flex gap-2 items-center">
                                Community
                            </span>
                            <span class="flex gap-2 items-center">
                                Find Ableton Users Groups
                                <ChevronRight :size="16"/>
                            </span>
                            <span class="flex gap-2 items-center">
                                Find Certified Training
                                <ChevronRight :size="16"/>
                            </span>
                            <span class="flex gap-2 items-center">
                                Become a Certified Trainer
                                <ChevronRight :size="16"/>
                            </span>
                        </div>
                        <div class="flex-1 flex gap-2 flex-col">
                            <span>
                                Distribution
                            </span>
                            <span class="flex gap-2 items-center">
                                Find Distributors
                                <ChevronRight :size="16"/>
                            </span>
                            <span class="flex gap-2 items-center">
                                Try Push in-store
                                <ChevronRight :size="16"/>
                            </span>
                        </div>
                        <div class="flex-1 flex gap-2 flex-col">
                            <span>
                                Language and Location
                            </span>
                            <div class="flex">
                                <select class="border" name="English">
                                    <option>
                                        English
                                    </option>
                                </select>
                                <select class="border" name="United States">
                                    <option>
                                        United States
                                    </option>
                                </select>
                            </div>
                        </div>
                    </div>
                    <div class="flex mt-10 justify-between">
                        <div class="flex gap-6">
                            <span>
                                Archive
                            </span>
                            <span>
                                Contact Us
                            </span>
                            <span>
                                Press Resources
                            </span>
                            <span>
                                Legal Info
                            </span>
                            <span>
                                Privacy Policy
                            </span>
                            <span>
                                Cookie Settings
                            </span>
                            <span>
                                Imprint
                            </span>
                        </div>
                        <div class="flex gap-4">
                            <div>
                               Made in Berlin 
                            </div>
                            <div class="flex">
                                <Menu />
                                <Columns3 />
                            </div>
                        </div>
                    </div>
                </footer>
            </main>
        </div>
    </div>
</template>

<script lang="ts" setup>
import { Facebook, Instagram, TwitterX, Youtube } from '@boxicons/vue';
import { ChevronRight, Columns3, Menu } from '@lucide/vue';
import Navbar from '~/components/navbar.vue';

</script>