#
# Copyright (C) 2014-2016 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
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

PKG_MAINTAINER:=Foo Bar <foo@bar>

include $(INCLUDE_DIR)/package.mk
include $(INCLUDE_DIR)/cmake.mk

CMAKE_OPTIONS += \
		 -DGUI=CLI \
		 -DVOIP=NO \
		 -DUSE_OWN_MBED_TLS=OFF

define Package/qaul
  SECTION:=net
  CATEGORY:=Network
  TITLE:=qaul
  DEPENDS:=
endef

$(eval $(call BuildPackage,qaul))
