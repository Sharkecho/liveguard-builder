include $(TOPDIR)/rules.mk

PKG_NAME:=liveguard-skeleton
PKG_RELEASE:=1

include $(INCLUDE_DIR)/package.mk

define Package/liveguard-skeleton
  SECTION:=net
  CATEGORY:=Network
  TITLE:=LiveGuard public integration skeleton
endef

define Package/liveguard-skeleton/description
Public packaging interface only; proprietary runtime components are not included.
endef

define Package/liveguard-skeleton/install
	$(INSTALL_DIR) $(1)/usr/share/liveguard
	$(INSTALL_DATA) ./README.public $(1)/usr/share/liveguard/README.public
endef

$(eval $(call BuildPackage,liveguard-skeleton))
