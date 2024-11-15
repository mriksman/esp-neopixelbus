idf_component_register(
    SRCS
        "NeoPixelBus/src/internal/HsbColor.cpp"
        "NeoPixelBus/src/internal/HslColor.cpp"
        "NeoPixelBus/src/internal/HtmlColor.cpp"
        "NeoPixelBus/src/internal/HtmlColorNames.cpp"
        "NeoPixelBus/src/internal/HtmlColorNameStrings.cpp"
        "NeoPixelBus/src/internal/HtmlColorShortNames.cpp"
        "NeoPixelBus/src/internal/NeoEsp32RmtMethod.cpp"
        "NeoPixelBus/src/internal/NeoGamma.cpp"
        "NeoPixelBus/src/internal/NeoPixelAnimator.cpp"
        "NeoPixelBus/src/internal/Rgb48Color.cpp"
        "NeoPixelBus/src/internal/RgbColor.cpp"
        "NeoPixelBus/src/internal/RgbColorBase.cpp"
        "NeoPixelBus/src/internal/RgbwColor.cpp"
        "NeoPixelBus/src/internal/SegmentDigit.cpp"
    INCLUDE_DIRS .
)

target_compile_definitions(${COMPONENT_TARGET} PRIVATE 
    "-DARDUINO_ARCH_ESP32")