#
# Copyright (C) 2015 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=youtube-dl
PKG_VERSION:=2019.6.27
PKG_RELEASE:=1

PKG_SOURCE:=youtube_dl-$(PKG_VERSION).tar.gz
PKG_SOURCE_URL:=https://files.pythonhosted.org/packages/source/y/youtube_dl/
PKG_HASH:=9ffbc02a0a150795f076b6a521fdfe2dad3f3305a8e3a0d29a720c551d4a9a44

PKG_BUILD_DIR:=$(BUILD_DIR)/youtube_dl-$(PKG_VERSION)

PKG_LICENSE:=Unlicense
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Adrian Panella <ianchi74@outlook.com>, Josef Schlehofer <pepe.schlehofer@gmail.com>

include $(INCLUDE_DIR)/package.mk
include ../../lang/python/python3-package.mk

define Package/youtube-dl/Default
  SECTION:=multimedia
  CATEGORY:=Multimedia
  TITLE:=Utility to download videos from YouTube.com
  URL:=https://yt-dl.org
  DEPENDS:=+ca-certificates
endef

define Package/youtube-dl/description
  youtube-dl is a small command-line program to download videos
  from YouTube.com and other video sites.
  It requires the Python3 interpreter.
endef

define Package/youtube-dl
$(call Package/youtube-dl/Default)
  DEPENDS+= \
    +python3 \
    +python3-email \
    +python3-xml \
    +python3-codecs \
    +python3-ctypes \
    +python3-setuptools
  VARIANT:=python3
endef

$(eval $(call Py3Package,youtube-dl))
$(eval $(call BuildPackage,youtube-dl))
$(eval $(call BuildPackage,youtube-dl-src))
