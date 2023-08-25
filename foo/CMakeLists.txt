set(TARGET foo-link)

# Set SOURCES variable
set(SOURCES
  foo.cpp
)

# Set HEADERS_PUBLIC variable (public headers, included in the library)
set(HEADERS_PUBLIC
  foo.h
)

# SHARED - target is found
add_library(${TARGET} SHARED ${SOURCES})

# SHARED - target is not found
#add_library(${TARGET} MODULE ${SOURCES})