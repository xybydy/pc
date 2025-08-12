# SPDX-License-Identifier: GPL-2.0-only
include $(TOPDIR)/rules.mk

PKG_NAME:=podman-compose
PKG_VERSION:=1.5.0
PKG_RELEASE:=1
PYPI_NAME:=podman-compose
PKG_HASH:=5cc09362852711ce5d27648e41cb5fd058ea5a75acbcdec2f8d0b0c114a18e8e

PKG_MAINTAINER:=xybydy
PKG_LICENSE:=GPL-3.0
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/$(PKG_NAME)
  SECTION:=utils
  CATEGORY:=Utilities
  SUBMENU:=Python
  TITLE:=Podman Compose
  URL:=https://github.com/containers/podman-compose
  DEPENDS:=+python3-light +python3-setuptools +python3-pyyaml +python3-requests
  VARIANT:=python3
endef

define Package/$(PKG_NAME)/description
  A script to help with managing pods using podman and docker-compose style YAML files.
endef

$(eval $(call Py3Package,$(PKG_NAME)))
$(eval $(call BuildPackage,$(PKG_NAME)))
