URL?=https://github.com/Loongson-Cloud-Community/tez/releases/download/0.9.2/webapp.tar.gz

download:
	@if [ ! -d "target" ]; then mkdir -p target; fi
	@wget -qO target/webapp.tar.gz $(URL)


remove-webapp:
	@rm -rf src/main/webapp

unpack: download remove-webapp
	@tar --extract \
		--file target/webapp.tar.gz \
		--directory "src/main"
	@rm -rf target/webapp.tar.gz
	
