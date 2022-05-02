cmake_minimum_required(VERSION 3.8.2)
project("ConsoleApp" LANGUAGES CSharp)

set(CMAKE_CSharp_FLAGS "/langversion:latest")

set_target_properties("test" PROPERTIES
    LINKER_LANGUAGE CSharp
    VS_DOTNET_TARGET_FRAMEWORK_VERSION "v4.5"
    VS_DOTNET_REFERENCES
        "Microsoft.CSharp;
        System;
        System.Core;
        System.Data;
        System.Data.DataSetExtensions"
)

add_subdirectory(ConsoleApp)