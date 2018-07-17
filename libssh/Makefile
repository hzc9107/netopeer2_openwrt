#
# This software is licensed under the Public Domain.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=libssh
PKG_VERSION:=0.7.5
PKG_RELEASE:=1

# see https://spdx.org/licenses/
PKG_LICENSE:=BSD-3-Clause
PKG_INSTALL:=1

PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://git.libssh.org/projects/libssh.git
PKG_SOURCE_VERSION:=afa4021ded6e58da4ee4d01dbf4e503d3711d002


include $(INCLUDE_DIR)/package.mk
include $(INCLUDE_DIR)/cmake.mk

define Package/libssh
	SECTION:=utils
	# Should this package be selected by default?
	#DEFAULT:=y
	CATEGORY:=Utilities
	TITLE:=Library to support ssh connectivity
	MAINTAINER:= Foo Bar <foo@example.com>
	URL:=https://git.libssh.org
	PKG_INSTALL_DIR:=$(1)/usr/local
endef

define Package/libssh/description
	Library to support ssh connectivity
endef

$(eval $(call BuildPackage,libssh))
