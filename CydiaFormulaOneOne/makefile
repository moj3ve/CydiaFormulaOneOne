ARCHS = armv7 arm64 armv7s 
TARGET = iphone:clang:9.0:7.0
include theos/makefiles/common.mk

BUNDLE_NAME = CydiaFormulaOneOne
CydiaFormulaOneOne_FILES = CydiaFormulaOneOne.mm
CydiaFormulaOneOne_INSTALL_PATH = /Library/PreferenceBundles
CydiaFormulaOneOne_FRAMEWORKS = UIKit
CydiaFormulaOneOne_PRIVATE_FRAMEWORKS = Preferences

include $(THEOS_MAKE_PATH)/bundle.mk

internal-stage::
	$(ECHO_NOTHING)mkdir -p $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences$(ECHO_END)
	$(ECHO_NOTHING)cp entry.plist $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences/CydiaFormulaOneOne.plist$(ECHO_END)
