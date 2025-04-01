---
template: home.html
title: V4 Api Reference & Documentation
hide:
  - toc
  - navigation
  - header
---
<h1 style="position: absolute"></h1>


<div id="app"></div>
<!-- Load Scalar and initialize it directly -->
<script>
    // Define configuration first
    var configuration = {
        theme: 'alternate',
        // Do not use the default fonts from the Scalar CDN
        withDefaultFonts: 'false',
    };
    
    function loadScalar() {
        var script = document.createElement('script');
        script.src = 'https://cdn.jsdelivr.net/npm/@scalar/api-reference';
        script.onload = function() {
            // Initialize immediately after script loads
            Scalar.createApiReference('#app', {
                // The URL of the OpenAPI/Swagger document
                url: '/assets/v4.yaml',
                // Avoid CORS issues
                proxyUrl: 'https://proxy.scalar.com',
            });
        };
        document.head.appendChild(script);
    }
    
    loadScalar();
</script>

<style>
:root {
    --scalar-font: 'Phantom Sans'
  }
  .dark-mode {
    --scalar-color-1: rgba(255, 255, 255, 0.81);
    --scalar-color-2: rgba(255, 255, 255, 0.443);
    --scalar-color-3: rgba(255, 255, 255, 0.282);
    --scalar-color-accent: #8ab4f8;
    --scalar-background-1: #17171D;
    --scalar-background-2:rgb(42, 39, 45);
    --scalar-background-3:rgb(52, 50, 58);
    --scalar-background-accent: #8ab4f81f;
  }
  .light-mode {
    --scalar-color-1: rgba(255, 255, 255, 0.81);
    --scalar-color-2: rgba(255, 255, 255, 0.443);
    --scalar-color-3: rgba(255, 255, 255, 0.282);
    --scalar-color-accent: #8ab4f8;
    --scalar-background-1: #17171D;
    --scalar-background-2:rgb(42, 39, 45);
    --scalar-background-3:rgb(52, 50, 58);
    --scalar-background-accent: #8ab4f81f;
  }
  .darklight-reference[data-v-c3203d44] {
    display: none;
  }
</style>