FLAGS+=' -fPIC'
CXXFLAGS+=' -fPIC'
export CFLAGS CXXFLAGS &&

USE_SYSTEM_LIBS='yes'
export USE_SYSTEM_LIBS &&

OPTS="prefix=/usr build=release CURL_LIBS='-lcurl -lpthread'"

default_make &&

install -Dm644 $SCRIPT_DIRECTORY/mupdf.desktop /usr/share/applications/mupdf.desktop &&
install -Dm644 $SCRIPT_DIRECTORY/mupdf.xpm /usr/share/pixmaps/mupdf.xpm &&

ln -sf /usr/bin/mupdf-x11 /usr/bin/mupdf
