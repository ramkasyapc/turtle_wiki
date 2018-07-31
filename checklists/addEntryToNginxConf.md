* 
Add the following snippet, it tells nginx to redirect /api/rnr/ to below proxy 
        location /api/rnr/ {
        proxy_pass      http://localhost:7010/api/rnr/;
        proxy_set_header xhost $host;
        }
