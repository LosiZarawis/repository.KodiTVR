.DEFAULT_GOAL := default
proj = "plugin.video.KodiTVR_Streams"
version = "0.0.8"

default:
	git archive --prefix=$(proj)/ master -o $(proj)-$(version).zip

install:
	git ls-files --others --exclude-standard --cached  | zip --names-stdin latest.zip
	unzip -o latest.zip -d ~/.kodi/addons/${proj}

clean:
	rm *.zip *.pyc
