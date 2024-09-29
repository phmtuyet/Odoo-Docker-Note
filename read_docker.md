# BASIC COMMAND
- Dowload images 

    `docker pull <image-Name>`

- Run images, download images nếu chưa có images (= pull + start)
	`docker run <image-NAME>`
	`docker run -d <image-NAME>`	( -d : detached mode)
- Check list images `docker images`
- Check list container `docker ps`

# NOTE FOR LINUX

- Docker trên ubuntu có thể có nhiều context, mỗi context như 1 user docker riêng quản lý các container, images khác nhau. Thông thường có 2 context là `default` và `destop-linux`. Mặc định là default, đó là lý do khi pull images bằng cmd, không thể thấy được images đó trên docker desktop. Vậy nên khi sử dụng docker bằng cmd chuyển context sang `desktop-linux`.
- Danh sách context docker: 	
	
    `docker context ls`
- Đổi context:
	
    `docker context use <docker-NAME>`

