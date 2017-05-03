How to build
============

.. code::
	cd lede
	echo 'src-git qaulfeed https://github.com/qaul/lede_feed.git' >> feeds.conf
	./scripts/feeds update
	./scripts/feeds install -p qaulfeed qaul
	make menuconfig
	# under Network -> qaul
	make package/qaul/compile
