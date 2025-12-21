.PHONY: build
build: _site/favicon.ico
	mkdir -p _site
	cat index.html > _site/index.html
	cat style.css > _site/style.css
	cat ../tree.gif > _site/tree.gif
	cat ../2024-ascii-christmas-tree > _site/2024
	cat ../2025-ascii-christmas-tree > _site/2025
	ln -sf 2025 _site/index.txt

_site/favicon.ico:
	mkdir -p _site
	curl -o _site/favicon.ico https://ysap.sh/favicon.ico

.PHONY: serve
serve:
	python3 -mhttp.server -d _site

# deploy the website
.PHONY: deploy
deploy: _site/favicon.ico
	rsync -avh --delete --progress \
	    ./_site/ web:/var/www/xmas.ysap.sh/
