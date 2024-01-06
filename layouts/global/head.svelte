<script>
  export let title, env;
</script>

<head>
  <meta charset="utf-8" />
  <meta http-equiv="X-UA-Compatible" content="IE=edge" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <base href="{env.baseurl}" />
  <!--Swap our for actual link-->
  <link rel="canonical" href="https://www.website.com/" />

  <meta name="description" content="Meta description for the page" />
  <meta name="keywords" content="" />

  <!--Social Media Display-->
  <meta property="og:title" content="Title that shows up on google searches" />
  <meta property="og:description" content="Meta description for the page" />
  <meta property="og:type" content="website" />
  <meta
    property="og:url"
    content="Official link for that page (https://www.site.com)"
  />
  <meta property="og:image" content="media/images/social.jpg" />
  <meta property="og:image:secure_url" content="media/images/social.jpg" />

  <!--Favicons-->
  <link
    rel="apple-touch-icon"
    sizes="180x180"
    href="media/favicons/apple-touch-icon.png"
  />
  <link
    rel="icon"
    type="image/png"
    sizes="32x32"
    href="media/favicons/favicon-32x32.png?v1"
  />
  <link
    rel="icon"
    type="image/png"
    sizes="16x16"
    href="media/favicons/favicon-16x16.png"
  />
  <link rel="manifest" href="media/favicons/site.webmanifest" />
  <meta name="msapplication-TileColor" content="#da532c" />
  <meta name="theme-color" content="#ffffff" />

  <title>{title} | CodeStitch</title>
  <!-- <base href={env.baseurl} /> -->
  <script type="module" src={`${env.entrypointJS}/core/main.js`}></script>
  <link rel='stylesheet' href={`${env.entrypointJS}/bundle.css`}>
  <link rel="icon" type="image/svg+xml" href="media/logo.svg" />
  <link rel="stylesheet" href="global.css" />
  <link
    rel="preload"
    href="fonts/roboto-v29-latin-regular.woff2 "
    as="font"
    type="font/woff2"
    crossorigin
  />
</head>
