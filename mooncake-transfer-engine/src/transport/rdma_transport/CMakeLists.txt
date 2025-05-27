file(GLOB RDMA_SOURCES "*.cpp")

add_library(rdma_transport OBJECT ${RDMA_SOURCES})
target_link_libraries(rdma_transport PRIVATE ${JSONCPP_LIBRARIES} glog::glog pthread)
