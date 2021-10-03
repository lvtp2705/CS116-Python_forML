Bước 1: Cài đặt các thư viện cần thiết

!pip install matplotlib==3.1.3
!pip install osmnet
!pip install folium

!pip install rtree
!pip install pygeos
!pip install geojson
!pip install geopandas



Bước 2: clone data từ https://github.com/CityScope/CSL_HCMC

Bước 3: Load ranh giới quận huyện và dân số quận huyện từ: Data\GIS\Population\population_HCMC\population_shapefile\Population_District_Level.shp

Bước 4: Load dữ liệu click của người dùng

Bước 5: Lọc ra 10 quận huyện có tốc độ tăng dân số nhanh nhất (Pop2019/Pop2017)

Bước 6: Dùng spatial join (from geopandas.tools import sjoin) để lọc ra các điểm click của người dùng trong 5 quận/huyện hot nhất

Bước 7: chạy KMean cho top 10 quận huyện này. Lấy K = 20

Bước 8: Lưu cụm điểm nhiều nhất của mỗi quận

Bước 9: show lên bản đồ các cụm đông nhất theo từng quận theo dạng HEATMAP

Bước 10: Lưu heatmap xuống file png
