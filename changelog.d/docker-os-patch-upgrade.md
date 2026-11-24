   ---
   bump: patch
   title: Docker image now applies latest Debian security patches on every build
   ---
   ## vi
   ### Bảo mật
   - **Ảnh Docker luôn vá OS mới nhất khi build lại.** Thêm `apt-get upgrade -y` ngay sau khi lấy ảnh nền, để các gói hệ thống (openssl, sqlite3, expat, ncurses...) không còn kẹt ở bản vá cũ do cache lớp ảnh nền.

   ## en
   ### Security
   - **Docker image now applies the latest Debian security patches on rebuild.** Added `apt-get upgrade -y` right after pulling the base image so system packages (openssl, sqlite3, expat, ncurses...) no longer stay stuck on a stale patch level from a cached base layer.
   
