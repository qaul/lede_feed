#
# qaul.net is free software
# licensed under GPL (version 3)
#


include $(TOPDIR)/rules.mk

PKG_NAME:=qaul
PKG_RELEASE:=1

PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL=https://github.com/qaul/qaul.net.git
PKG_SOURCE_DATE:=2017-05-03
PKG_SOURCE_VERSION:=a653d44badad5cf0c708ae53da41992578b38338
CMAKE_INSTALL:=1

PKG_LICENSE:=GPL-3.0
PKG_LICENSE_FILES:=

PKG_MAINTAINER:=qaul.net community <contact@qaul.net>

include $(INCLUDE_DIR)/package.mk
include $(INCLUDE_DIR)/cmake.mk

CMAKE_OPTIONS += \
		 -DGUI=CLI \
		 -DVOIP=NO \
		 -DUSE_SYSTEM_MBEDTLS=YES

define Package/qaul
  SECTION:=net
  CATEGORY:=Network
  TITLE:=qaul.net
  DEPENDS:=+olsr +mbedtls
endef

$(eval $(call BuildPackage,qaul))
