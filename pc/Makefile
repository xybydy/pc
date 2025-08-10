# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=podman-compose
PKG_VERSION:=1.5.0
PKG_RELEASE:=1

PYPI_NAME:=podman-compose
PKG_HASH:=5cc09362852711ce5d27648e41cb5fd058ea5a75acbcdec2f8d0b0c114a18e8e


include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/podman-compose
  SECTION:=utils
  CATEGORY:=Utilities
  TITLE:=Podman Compose
  URL:=https://podman.io
  DEPENDS:=+python3-light +podman
endef

define Package/podman-compose/description
  Podman Compose
endef

$(eval $(call Py3Package,podman-compose))
$(eval $(call BuildPackage,podman-compose))
$(eval $(call BuildPackage,podman-compose-src))