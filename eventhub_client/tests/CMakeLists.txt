#Copyright (c) Microsoft. All rights reserved.
#Licensed under the MIT license. See LICENSE file in the project root for full license information.

cmake_minimum_required(VERSION 2.8.11)

#this is CMakeLists for the eventhub_client tests folder

add_subdirectory(eventdata_unittests)
add_subdirectory(eventhubclient_unittests)
add_subdirectory(eventhubclient_ll_unittests)
add_subdirectory(eventhubreceiver_unittests)
add_subdirectory(eventhubreceiver_ll_unittests)
add_subdirectory(eventhubauth_unittests)
add_subdirectory(kvp_parser_unittests)
if (${run_e2e_tests})
    #add_subdirectory(eventhubclient_e2etests)
endif()
