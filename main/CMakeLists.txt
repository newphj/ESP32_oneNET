
file(GLOB_RECURSE srcs ../componnects/app/src/*.c ../componnects/oneNET_token/*.c )

idf_component_register(SRCS "main.c" ${srcs}
                    INCLUDE_DIRS "." ../componnects/app/include  ../componnects/oneNET_token ../componnects/oneNET_token/cipher   
                    )
