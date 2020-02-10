# libnl-3.4.0
Introduction to libnl
The libnl suite is a collection of libraries providing APIs to netlink protocol based Linux kernel interfaces.

This package is known to build and work properly using an LFS-9.0 platform.
Installation of libnl
Install libnl by running the following commands:

./configure --prefix=/usr     \
            --sysconfdir=/etc \
            --disable-static  &&
make
To test the results, issue: make check.

Now, as the root user:

make install
If you wish to install the API documentation, as the root user:

mkdir -vp /usr/share/doc/libnl-3.4.0 &&
tar -xf ../libnl-doc-3.4.0.tar.gz --strip-components=1 --no-same-owner \
    -C  /usr/share/doc/libnl-3.4.0
Command Explanations
--disable-static: This switch prevents installation of static versions of the libraries.

--disable-cli: Use this parameter if you don't want to install cli tools provided by the package.

Contents
Installed Programs:
genl-ctrl-list, idiag-socket-details, nl-class-add, nl-class-delete, nl-classid-lookup, nl-class-list, nl-cls-add, nl-cls-delete, nl-cls-list, nl-link-list, nl-pktloc-lookup, nl-qdisc-add, nl-qdisc-delete, nl-qdisc-list, and 32 other helper programs with nl- and nf- prefixes
Installed Libraries:
libnl-3.so, libnl-cli-3.so, libnl-genl-3.so, libnl-idiag-3.so, libnl-nf-3.so, libnl-route-3.so, libnl-xfrm-3.so, and cli modules under /usr/lib/libnl/cli tree
Installed Directories:
/etc/libnl, /usr/include/libnl3, /usr/lib/libnl, and /usr/share/doc/libnl-3.4.0
Short Descriptions
genl-ctrl-list

queries the Generic Netlink controller in the kernel and prints a list of all registered Generic Netlink families including the version of the interface that has been registered.

nl-class-add

adds, updates, or replaces Traffic Classes

nl-class-delete

deletes Traffic Classes

nl-classid-lookup

is used to resolve qdisc/class names to classid values and vice versa.

nl-class-list

lists Traffic Classes.

nl-cls-add

adds a classifier.

nl-cls-delete

deletes a classifier.

nl-cls-list

lists classifiers.

nl-link-list

dumps link attributes.

nl-pktloc-lookup

allows the lookup of packet location definitions.

nl-qdisc-add

adds queueing disciplines (qdiscs) in the kernel.

nl-qdisc-delete

deletes queueing disciplines (qdiscs) in the kernel.

nl-qdisc-list

lists queueing disciplines (qdiscs) in the kernel.

libnl*-3.so

These libraries contain API functions used to access Netlink interfaces in Linux kernel.

Last updated on 2019-08-16 20:46:23 -0700
