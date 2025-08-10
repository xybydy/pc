# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=podman-compose
PKG_VERSION:=1.5.0
PKG_RELEASE:=1

PKG_SOURCE:=podman_compose-$(PKG_VERSION).tar.gz
PKG_SOURCE_URL:=https://files.pythonhosted.org/packages/24/91/b168a685ca6813ff9b467d76a7365a099aec16a1032b6edf39b0cd19f6c3
PKG_HASH:=5cc09362852711ce5d27648e41cb5fd058ea5a75acbcdec2f8d0b0c114a18e8e
PKG_BUILD_DIR:=$(BUILD_DIR)/setools

PKG_LICENSE:=GPL-2.0-only


include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/podman-compose
  SECTION:=utils
  CATEGORY:=Utilities
  TITLE:=Podman Compose
  URL:=https://podman.io
  DEPENDS:=+python3 +podman
endef

define Package/podman-compose/description
  Podman Compose
endef

$(eval $(call Py3Package,podman-compose))
$(eval $(call BuildPackage,podman-compose))