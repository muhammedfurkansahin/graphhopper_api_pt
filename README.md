# graphhopper_public_transportation


⸻

English Description

🚀 Overview

This project provides a customized Docker image of the GraphHopper routing engine with integrated OpenStreetMap (OSM) and GTFS data for Turkey. It supports walking, car, and public transport modes using the Dijkstra algorithm for route calculations, including alternative routes. ￼

🧩 Features
	•	Integration of OSM data for Turkey using turkey-latest.osm.bz2
	•	Public transport integration with GTFS data
	•	Support for walking, car, and public transport modes
	•	Route calculations using the Dijkstra algorithm
	•	Provision of alternative routes
	•	Support for both x86_64 and ARM architectures

📦 Docker Image

Pull the Docker image using the following command: ￼

docker pull ghcr.io/muhammedfurkansahin/graphhopper-navigation-api-x86-64:latest

⚙️ Usage

Run the Docker container as follows: ￼

docker run -d -p 8989:8989 \
  -v $(pwd)/data:/data \
  ghcr.io/muhammedfurkansahin/graphhopper-navigation-api-x86-64:latest

Place your turkey-latest.osm.bz2 and GTFS files into the /data directory.

🛠 Configuration

Configure the config.yml file with the following settings: ￼
	•	graphhopper.datareader.file: OSM data file
	•	graphhopper.gtfs.file: GTFS data file
	•	graphhopper.graph.location: Location to store graph data
	•	graphhopper.profiles: Profile types to use (e.g., car, foot, pt) ￼

📄 License

This project is built upon the open-source contributions of the GraphHopper community.
⸻

GraphHopper Navigation API (x86_64 & ARM)

Türkçe Açıklama

🚀 Genel Bakış

Bu proje, GraphHopper yönlendirme motorunun özelleştirilmiş bir Docker imajını sunar. Türkiye geneli için OpenStreetMap (OSM) ve GTFS verileri entegre edilmiştir. Yürüyüş, araba ve toplu taşıma modları için Dijkstra algoritması kullanılarak rota hesaplamaları yapılır. Alternatif rotalar da desteklenmektedir.

🧩 Özellikler
	•	Türkiye geneli için turkey-latest.osm.bz2 dosyasıyla OSM verisi entegrasyonu
	•	GTFS verisi ile toplu taşıma entegrasyonu
	•	Yürüyüş, araba ve toplu taşıma modları için destek
	•	Dijkstra algoritması kullanılarak rota hesaplamaları
	•	Alternatif rotaların sunulması
	•	x86_64 ve ARM mimarileri için destek

📦 Docker İmajı

Docker imajını aşağıdaki komutla çekebilirsiniz:

docker pull ghcr.io/muhammedfurkansahin/graphhopper-navigation-api-x86-64:latest

⚙️ Kullanım

Docker konteynerini aşağıdaki şekilde çalıştırabilirsiniz:

docker run -d -p 8989:8989 \
  -v $(pwd)/data:/data \
  ghcr.io/muhammedfurkansahin/graphhopper-navigation-api-x86-64:latest

/data klasörüne turkey-latest.osm.bz2 ve GTFS dosyalarınızı yerleştirin. ￼

🛠 Yapılandırma

config.yml dosyasında aşağıdaki ayarları yapabilirsiniz:
	•	graphhopper.datareader.file: OSM veri dosyası
	•	graphhopper.gtfs.file: GTFS veri dosyası
	•	graphhopper.graph.location: Graf verilerinin saklanacağı konum
	•	graphhopper.profiles: Kullanılacak profil türleri (örneğin, car, foot, pt) ￼ ￼

📄 Lisans

Bu proje, GraphHopper topluluğunun açık kaynak katkıları üzerine inşa edilmiştir.


⸻


'''
 __  __     _____           _                 ____        _     _       
|  \/  |   |  ___|   _ _ __| | ____ _ _ __   / ___|  __ _| |__ (_)_ __  
| |\/| |   | |_ | | | | '__| |/ / _` | '_ \  \___ \ / _` | '_ \| | '_ \ 
| |  | |_  |  _|| |_| | |  |   < (_| | | | |  ___) | (_| | | | | | | | |
|_|  |_(_) |_|   \__,_|_|  |_|\_\__,_|_| |_| |____/ \__,_|_| |_|_|_| |_|
                                                )__)                    
'''

