#
# This software is licensed under the Public Domain.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=libyang
PKG_VERSION:=0.15.146
PKG_RELEASE:=1

# see https://spdx.org/licenses/
PKG_LICENSE:=BSD-3-Clause
PKG_INSTALL:=1

PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/CESNET/libyang.git
PKG_SOURCE_VERSION:=572de240307bbba375b255b40e44ba148bd4b8d4


include $(INCLUDE_DIR)/package.mk
include $(INCLUDE_DIR)/cmake.mk

define Package/libyang
	SECTION:=utils
	# Should this package be selected by default?
	#DEFAULT:=y
	CATEGORY:=Utilities
	TITLE:=Library to support yang files parsing
	MAINTAINER:= Foo Bar <foo@example.com>
	URL:=https://github.com/CESNET/libyang
	PKG_INSTALL_DIR:=$(1)/usr/local
endef

define Package/libyang/description
	Library for parsing yang files
endef

$(eval $(call BuildPackage,libyang))
