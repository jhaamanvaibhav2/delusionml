add_library(delusionml SHARED
    core/tensor.cpp
)

target_link_libraries(delusionml
    PRIVATE
    ${METAL_LIBRARY}
    ${FOUNDATION_LIBRARY}
)