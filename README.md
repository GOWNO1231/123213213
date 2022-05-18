<!DOCTYPE html>
<html lang="en-US">
 
<head>
    <meta charset="UTF-8">
 
    <!-- Begin Jekyll SEO tag v2.8.0 -->
    <title>zmikolaj.github.io</title>
    <meta name="generator" content="Jekyll v3.9.2" />
    <meta property="og:title" content="zmikolaj.github.io" />
    <meta property="og:locale" content="en_US" />
    <link rel="canonical" href="https://grdoksm.github.io/grd.github.io/" />
    <meta property="og:url" content="https://grdoksm.github.io/grd.github.io/" />
    <meta property="og:site_name" content="grd.github.io" />
    <meta property="og:type" content="website" />
    <meta name="twitter:card" content="summary" />
    <meta property="twitter:title" content="grd.github.io" />
    <!-- End Jekyll SEO tag -->
 
    <link rel="preconnect" href="https://fonts.gstatic.com">
    <link rel="preload" href="https://fonts.googleapis.com/css?family=Open+Sans:400,700&display=swap" as="style" type="text/css" crossorigin>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="theme-color" content="#157878">
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <link rel="stylesheet" href="/grd.github.io/assets/css/style.css?v=7763892b7d1a980f2ec4b159a9ad3b7772c469ab">
    <!-- start custom head snippets, customize with your own _includes/head-custom.html file -->
 
    <!-- Setup Google Analytics -->
 
 
 
    <!-- You can set your favicon here -->
    <!-- link rel="shortcut icon" type="image/x-icon" href="/grd.github.io/favicon.ico" -->
 
    <!-- end custom head snippets -->
 
</head>
 
<body>
    <a id="skip-to-content" href="#content">Skip to the content.</a>
 
    <header class="page-header" role="banner">
        <h1 class="project-name">grd.github.io</h1>
        <h2 class="project-tagline"></h2>
 
        <a href="https://github.com/grdoksm/grd.github.io" class="btn">View on GitHub</a>
 
 
    </header>
 
    <main id="content" class="main-content" role="main">
        <p><!DOCTYPE html></p>
        <html lang="en">
 
        <head>
            <meta charset="UTF-8" />
            <meta name="viewport" content="width=device-width, initial-scale=1.0" />
            <style>
                * {
                    font-family: "Comic Sans MS", "Comic Sans";
                }
            </style>
            <title>LOLOLOLO</title>
        </head>
 
        <body>
            <h1>uwu</h1>
            <h2><input type="checkbox" class="catboy" />i am a catboy2</h2>
            <button class="napierdalacz">
                <img src="https://i.imgur.com/31fA5CM.png" width="100" height="100" />
            </button>
            <button class="napierdalacz-stop">
                <img src="https://i.imgur.com/sgQXzaw.png" width="100" height="100" alt="" />
            </button>
            <input type="number" class="loyalityId" value="985" />
            <script>
                let coupons = [
                    37125,
                    53279,
                    53705,
                    53742,
                    53746,
                    53748,
                    53765,
                    53801,
                    53802,
                    53803,
                    53804,
                    53805,
                    53806,
                    53807,
                    53808,
                    53809,
                    53810,
                ];
                let intid = null;
                var ax = 95944;
                document.querySelector(".napierdalacz").addEventListener("click", () => {
                    if (intid) clearInterval(intid);
 
                    intid = setInterval(() => {
                        getPrize(
                            mcd.bridge.message("offerActivation"),
                            parseInt(document.querySelector(".loyalityId").value)
                        );
                        ax--;
                        if (document.querySelector(".catboy").checked) {
                            document.querySelector(".loyalityId").value =
                                parseInt(document.querySelector(".loyalityId").value) - 1;
                        }
                    }, 1500);
                });
                document
                    .querySelector(".napierdalacz-stop")
                    .addEventListener("click", () => {
                        if (intid) clearInterval(intid);
                    });
                document.addEventListener("mcdBridgeReady", function(e) {
                    console.log(mcd);
                    let offerActivation = mcd.bridge.message("offerActivation");
                    let user = mcd.bridge.message("user");
                    user.send({
                        promptlogin: true
                    });
                    user.on("data", function(data) {
                        console.log(JSON.stringify(data));
                        //   getPrize(offerActivation);
                        let i = 985;
                    });
                    user.on("error", function(error) {});
                    user.on("done", function() {});
                });
 
                function getPrize(offerActivation, loyalityId) {
                    let couponId =
                        coupons[Math.floor(Math.random() * coupons.length) + 1 - 1];
 
                    offerActivation.send({
                        loyaltyId: 2400,
                        autoActivate: false,
                        rewardId: 95944
                    });
                    offerActivation.on("data", function(data) {
                        console.log("offer activation data", loyalityId, data);
                    });
                    offerActivation.on("error", function(error) {
                        console.warn("MCD ERROR", loyalityId, JSON.stringify(error));
                    });
                    offerActivation.on("done", function() {
                        console.log("corn done", loyalityId);
                    });
                }
 
                function getPrize2(offerActivation, loyalityId, i) {
                    let couponId =
                        coupons[Math.floor(Math.random() * coupons.length) + 1 - 1];
 
                    offerActivation.send({
                        loyaltyId: 2400,
                        autoActivate: false,
                        rewardId: ax
                    });
                    offerActivation.on("data", function(data) {
                        console.log("offer activation data", loyalityId, data);
                    });
                    offerActivation.on("error", function(error) {
                        console.warn("MCD ERROR", loyalityId, JSON.stringify(error));
                    });
                    offerActivation.on("done", function() {
                        console.log("corn done", loyalityId);
                    });
                }
            </script>
            <script src="//cdn.jsdelivr.net/npm/eruda"></script>
            <script>
                eruda.init();
            </script>
        </body>
 
        </html>
 
 
        <footer class="site-footer">
 
            <span class="site-footer-owner"><a href="https://github.com/grdoksm/grd.github.io">grd.github.io</a> is maintained by <a href="https://github.com/grdoksm">grdoksm</a>.</span>
 
            <span class="site-footer-credits">This page was generated by <a href="https://pages.github.com">GitHub Pages</a>..</span>
        </footer>
    </main>
</body>
 
</html>
