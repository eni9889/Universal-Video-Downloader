TARGET=iphone:clang:latest:6.0
THEOS_DEVICE_PORT=22
GO_EASY_ON_ME=1
export ARCHS = armv7 armv7s arm64

include $(THEOS)/makefiles/common.mk

TWEAK_NAME = UniversalVideoDownloader
UniversalVideoDownloader_FILES = UVDListener.xm UVDAlertViewHandler.m UVDVideoProcessor.m UVDAuthenticationDialog.m UVDDataCompressor.m UVDDataDecompressor.m UVDHTTPRequest.m UVDInputStream.m UVDReachability.m
UniversalVideoDownloader_FRAMEWORKS = UIKit Foundation AVFoundation MediaPlayer CFNetwork SystemConfiguration MobileCoreServices CoreGraphics
UniversalVideoDownloader_LDFLAGS = -lz

include $(THEOS_MAKE_PATH)/tweak.mk