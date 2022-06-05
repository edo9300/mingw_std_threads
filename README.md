# mingw_std-threads
Adding mingw std::thread in c++11/14. Patch mingw is included in &lt;thread>, &lt;mutex>, &lt;future> files. The added mingw invoke function is only for thread. It contains variations of the &lt;type_traits> library. So don't add mingw.invoke.h to change only for &lt;type_traits>, &lt;utility>, &lt;functional>. The mingw.future.h function doesn't start packaged_task. This function is extensive and would rewrite function for mingw std::thread.