set(PK3DIRS
    scripts
    models
    gfx
    menu
    textures
    maps
    music
)
compress_pk3(xmas ${PK3DIRS})

set(SHADERS
    monsterpad.shader
    pad_garden.shader
    padmodel.shader
    wop_xmas.shader
)
foreach (SHADER ${SHADERS})
    shader_validation(xmas ${SHADER} 0)
endforeach()

set(BSPS
    weinacht.bsp
)
foreach (BSP ${BSPS})
    bsp_validation(xmas ${BSP} 0)
endforeach()
