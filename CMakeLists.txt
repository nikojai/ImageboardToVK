cmake_minimum_required(VERSION 3.26.4)
project(ImagebordToVK VERSION 0.1.0 LANGUAGES CXX)
set (CMAKE_CXX_STANDARD 20) 

set(CMAKE_PREFIX_PATH "C:/repos/CURL;C:/repos/zlib;C:/repos/cpr;C:/repos/httplib;C:/repos/nlohmann_json")

find_package(httplib REQUIRED)
find_package(nlohmann_json REQUIRED)
find_package(cpr REQUIRED)
find_package(CURL REQUIRED)
find_package(inja REQUIRED)

add_executable(ImagebordToVK
    # Тут будут файлы кода проекта.
)


# For libraries with configs
target_link_libraries(ImagebordToVK nlohmann_json::nlohmann_json cpr::cpr httplib::httplib pantor::inja CURL::libcurl)