add_library(boost_serialization INTERFACE)
add_library(Boost::serialization ALIAS boost_serialization)
target_include_directories(boost_serialization INTERFACE include)
target_link_libraries(boost_serialization
        INTERFACE
        Boost::array
        Boost::assert
        Boost::config
        Boost::core
        Boost::detail
        Boost::integer
        Boost::io
        Boost::iterator
        Boost::move
        Boost::mpl
        Boost::optional
        Boost::predef
        Boost::preprocessor
        Boost::smart_ptr
        Boost::static_assert
        Boost::type_traits
        Boost::unordered
        Boost::utility
        Boost::variant
        )
