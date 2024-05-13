**NanoHTTP: Lightweight yet Powerful HTTP Server in Rust**

NanoHTTP aims to provide a compact yet robust HTTP server in Rust. Its primary goals are to adhere fully to the HTTP standard and to offer a simple approach to building HTTP servers.

**What tasks does NanoHTTP manage?**
- Accepting and managing client connections
- Parsing HTTP requests
- Supporting HTTP requests pipelining
- Providing HTTPS support (utilizing OpenSSL, Rustls, or native-tls)
- Handling Transfer-Encoding and Content-Encoding
- Converting user input (e.g., POST data) into a contiguous UTF-8 string (*currently under development*)
- Handling Range requests (*currently under development*)
- Supporting `Connection: upgrade` (used for websockets)

NanoHTTP handles all aspects related to client connections, data transfer, and encoding.

However, it leaves other tasks, such as parsing header values, handling multipart data, routing, etags, cache-control, HTML templates, etc., to be managed by your code.
If you intend to develop a website in Rust, it's advisable to use a comprehensive framework instead of relying solely on this library.
