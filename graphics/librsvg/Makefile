# $NetBSD: Makefile,v 1.123 2020/06/14 15:33:27 nia Exp $

DISTNAME=	librsvg-2.48.3
PKGREVISION=	1
CATEGORIES=	graphics gnome
MASTER_SITES=	${MASTER_SITE_GNOME:=sources/librsvg/${PKGVERSION_NOREV:R}/}
EXTRACT_SUFX=	.tar.xz

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://wiki.gnome.org/LibRsvg
COMMENT=	SVG library for GNOME
LICENSE=	gnu-lgpl-v2.1

MAKE_JOBS_SAFE=	NO
MAKE_FLAGS+=	CARGO_MAKE_JOBS=-j${_MAKE_JOBS_N}

USE_LIBTOOL=		yes
USE_TOOLS+=		pkg-config gmake aclocal autoconf automake
USE_LANGUAGES+=		c c++
GNU_CONFIGURE=		yes
CONFIGURE_ARGS+=	--disable-tools
#CONFIGURE_ARGS+=	--enable-Bsymbolic=auto
CONFIGURE_ARGS+=	--disable-Bsymbolic

PKGCONFIG_OVERRIDE=	librsvg.pc.in

TEST_TARGET=		check

CARGO_CRATE_DEPENDS+=	aho-corasick-0.7.10
CARGO_CRATE_DEPENDS+=	alga-0.9.3
CARGO_CRATE_DEPENDS+=	approx-0.3.2
CARGO_CRATE_DEPENDS+=	atty-0.2.14
CARGO_CRATE_DEPENDS+=	autocfg-1.0.0
CARGO_CRATE_DEPENDS+=	bitflags-1.2.1
CARGO_CRATE_DEPENDS+=	block-0.1.6
CARGO_CRATE_DEPENDS+=	bstr-0.2.12
CARGO_CRATE_DEPENDS+=	byteorder-1.3.4
CARGO_CRATE_DEPENDS+=	cairo-rs-0.8.1
CARGO_CRATE_DEPENDS+=	cairo-sys-rs-0.9.2
CARGO_CRATE_DEPENDS+=	cast-0.2.3
CARGO_CRATE_DEPENDS+=	cfg-if-0.1.10
CARGO_CRATE_DEPENDS+=	clap-2.33.0
CARGO_CRATE_DEPENDS+=	cloudabi-0.0.3
CARGO_CRATE_DEPENDS+=	criterion-0.2.11
CARGO_CRATE_DEPENDS+=	criterion-plot-0.3.1
CARGO_CRATE_DEPENDS+=	crossbeam-deque-0.7.3
CARGO_CRATE_DEPENDS+=	crossbeam-epoch-0.8.2
CARGO_CRATE_DEPENDS+=	crossbeam-queue-0.2.1
CARGO_CRATE_DEPENDS+=	crossbeam-utils-0.7.2
CARGO_CRATE_DEPENDS+=	cssparser-0.27.2
CARGO_CRATE_DEPENDS+=	cssparser-macros-0.6.0
CARGO_CRATE_DEPENDS+=	csv-1.1.3
CARGO_CRATE_DEPENDS+=	csv-core-0.1.10
CARGO_CRATE_DEPENDS+=	data-url-0.1.0
CARGO_CRATE_DEPENDS+=	derive_more-0.99.5
CARGO_CRATE_DEPENDS+=	downcast-rs-1.1.1
CARGO_CRATE_DEPENDS+=	dtoa-0.4.5
CARGO_CRATE_DEPENDS+=	dtoa-short-0.3.2
CARGO_CRATE_DEPENDS+=	either-1.5.3
CARGO_CRATE_DEPENDS+=	encoding-0.2.33
CARGO_CRATE_DEPENDS+=	encoding-index-japanese-1.20141219.5
CARGO_CRATE_DEPENDS+=	encoding-index-korean-1.20141219.5
CARGO_CRATE_DEPENDS+=	encoding-index-simpchinese-1.20141219.5
CARGO_CRATE_DEPENDS+=	encoding-index-singlebyte-1.20141219.5
CARGO_CRATE_DEPENDS+=	encoding-index-tradchinese-1.20141219.5
CARGO_CRATE_DEPENDS+=	encoding_index_tests-0.1.4
CARGO_CRATE_DEPENDS+=	float-cmp-0.6.0
CARGO_CRATE_DEPENDS+=	fuchsia-cprng-0.1.1
CARGO_CRATE_DEPENDS+=	futf-0.1.4
CARGO_CRATE_DEPENDS+=	futures-channel-0.3.4
CARGO_CRATE_DEPENDS+=	futures-core-0.3.4
CARGO_CRATE_DEPENDS+=	futures-executor-0.3.4
CARGO_CRATE_DEPENDS+=	futures-io-0.3.4
CARGO_CRATE_DEPENDS+=	futures-macro-0.3.4
CARGO_CRATE_DEPENDS+=	futures-task-0.3.4
CARGO_CRATE_DEPENDS+=	futures-util-0.3.4
CARGO_CRATE_DEPENDS+=	fxhash-0.2.1
CARGO_CRATE_DEPENDS+=	gdk-pixbuf-0.8.0
CARGO_CRATE_DEPENDS+=	gdk-pixbuf-sys-0.9.1
CARGO_CRATE_DEPENDS+=	generic-array-0.13.2
CARGO_CRATE_DEPENDS+=	getrandom-0.1.14
CARGO_CRATE_DEPENDS+=	gio-0.8.1
CARGO_CRATE_DEPENDS+=	gio-sys-0.9.1
CARGO_CRATE_DEPENDS+=	glib-0.9.3
CARGO_CRATE_DEPENDS+=	glib-sys-0.9.1
CARGO_CRATE_DEPENDS+=	gobject-sys-0.9.1
CARGO_CRATE_DEPENDS+=	hermit-abi-0.1.10
CARGO_CRATE_DEPENDS+=	idna-0.2.0
CARGO_CRATE_DEPENDS+=	itertools-0.8.2
CARGO_CRATE_DEPENDS+=	itoa-0.4.5
CARGO_CRATE_DEPENDS+=	language-tags-0.2.2
CARGO_CRATE_DEPENDS+=	lazy_static-1.4.0
CARGO_CRATE_DEPENDS+=	libc-0.2.68
CARGO_CRATE_DEPENDS+=	libm-0.2.1
CARGO_CRATE_DEPENDS+=	locale_config-0.3.0
CARGO_CRATE_DEPENDS+=	log-0.4.8
CARGO_CRATE_DEPENDS+=	mac-0.1.1
CARGO_CRATE_DEPENDS+=	malloc_buf-0.0.6
CARGO_CRATE_DEPENDS+=	markup5ever-0.10.0
CARGO_CRATE_DEPENDS+=	matches-0.1.8
CARGO_CRATE_DEPENDS+=	matrixmultiply-0.2.3
CARGO_CRATE_DEPENDS+=	maybe-uninit-2.0.0
CARGO_CRATE_DEPENDS+=	memchr-2.3.3
CARGO_CRATE_DEPENDS+=	memoffset-0.5.4
CARGO_CRATE_DEPENDS+=	nalgebra-0.19.0
CARGO_CRATE_DEPENDS+=	new_debug_unreachable-1.0.4
CARGO_CRATE_DEPENDS+=	nodrop-0.1.14
CARGO_CRATE_DEPENDS+=	num-complex-0.2.4
CARGO_CRATE_DEPENDS+=	num-integer-0.1.42
CARGO_CRATE_DEPENDS+=	num-rational-0.2.4
CARGO_CRATE_DEPENDS+=	num-traits-0.2.11
CARGO_CRATE_DEPENDS+=	num_cpus-1.12.0
CARGO_CRATE_DEPENDS+=	objc-0.2.7
CARGO_CRATE_DEPENDS+=	objc-foundation-0.1.1
CARGO_CRATE_DEPENDS+=	objc_id-0.1.1
CARGO_CRATE_DEPENDS+=	once_cell-1.3.1
CARGO_CRATE_DEPENDS+=	pango-0.8.0
CARGO_CRATE_DEPENDS+=	pango-sys-0.9.1
CARGO_CRATE_DEPENDS+=	pangocairo-0.9.0
CARGO_CRATE_DEPENDS+=	pangocairo-sys-0.10.1
CARGO_CRATE_DEPENDS+=	percent-encoding-2.1.0
CARGO_CRATE_DEPENDS+=	phf-0.8.0
CARGO_CRATE_DEPENDS+=	phf_codegen-0.8.0
CARGO_CRATE_DEPENDS+=	phf_generator-0.8.0
CARGO_CRATE_DEPENDS+=	phf_macros-0.8.0
CARGO_CRATE_DEPENDS+=	phf_shared-0.8.0
CARGO_CRATE_DEPENDS+=	pin-utils-0.1.0-alpha.4
CARGO_CRATE_DEPENDS+=	pkg-config-0.3.17
CARGO_CRATE_DEPENDS+=	ppv-lite86-0.2.6
CARGO_CRATE_DEPENDS+=	precomputed-hash-0.1.1
CARGO_CRATE_DEPENDS+=	proc-macro-hack-0.5.15
CARGO_CRATE_DEPENDS+=	proc-macro-nested-0.1.4
CARGO_CRATE_DEPENDS+=	proc-macro2-1.0.10
CARGO_CRATE_DEPENDS+=	quote-1.0.3
CARGO_CRATE_DEPENDS+=	rand-0.7.3
CARGO_CRATE_DEPENDS+=	rand_chacha-0.2.2
CARGO_CRATE_DEPENDS+=	rand_core-0.3.1
CARGO_CRATE_DEPENDS+=	rand_core-0.4.2
CARGO_CRATE_DEPENDS+=	rand_core-0.5.1
CARGO_CRATE_DEPENDS+=	rand_distr-0.2.2
CARGO_CRATE_DEPENDS+=	rand_hc-0.2.0
CARGO_CRATE_DEPENDS+=	rand_os-0.1.3
CARGO_CRATE_DEPENDS+=	rand_pcg-0.2.1
CARGO_CRATE_DEPENDS+=	rand_xoshiro-0.1.0
CARGO_CRATE_DEPENDS+=	rawpointer-0.2.1
CARGO_CRATE_DEPENDS+=	rayon-1.3.0
CARGO_CRATE_DEPENDS+=	rayon-core-1.7.0
CARGO_CRATE_DEPENDS+=	rctree-0.3.3
CARGO_CRATE_DEPENDS+=	rdrand-0.4.0
CARGO_CRATE_DEPENDS+=	redox_syscall-0.1.56
CARGO_CRATE_DEPENDS+=	regex-1.3.6
CARGO_CRATE_DEPENDS+=	regex-automata-0.1.9
CARGO_CRATE_DEPENDS+=	regex-syntax-0.6.17
CARGO_CRATE_DEPENDS+=	rustc_version-0.2.3
CARGO_CRATE_DEPENDS+=	ryu-1.0.3
CARGO_CRATE_DEPENDS+=	same-file-1.0.6
CARGO_CRATE_DEPENDS+=	scopeguard-1.1.0
CARGO_CRATE_DEPENDS+=	selectors-0.22.0
CARGO_CRATE_DEPENDS+=	semver-0.9.0
CARGO_CRATE_DEPENDS+=	semver-parser-0.7.0
CARGO_CRATE_DEPENDS+=	serde-1.0.106
CARGO_CRATE_DEPENDS+=	serde_derive-1.0.106
CARGO_CRATE_DEPENDS+=	serde_json-1.0.51
CARGO_CRATE_DEPENDS+=	servo_arc-0.1.1
CARGO_CRATE_DEPENDS+=	siphasher-0.3.2
CARGO_CRATE_DEPENDS+=	slab-0.4.2
CARGO_CRATE_DEPENDS+=	smallvec-1.3.0
CARGO_CRATE_DEPENDS+=	stable_deref_trait-1.1.1
CARGO_CRATE_DEPENDS+=	string_cache-0.8.0
CARGO_CRATE_DEPENDS+=	string_cache_codegen-0.5.1
CARGO_CRATE_DEPENDS+=	syn-1.0.17
CARGO_CRATE_DEPENDS+=	tendril-0.4.1
CARGO_CRATE_DEPENDS+=	textwrap-0.11.0
CARGO_CRATE_DEPENDS+=	thin-slice-0.1.1
CARGO_CRATE_DEPENDS+=	thread_local-1.0.1
CARGO_CRATE_DEPENDS+=	time-0.1.42
CARGO_CRATE_DEPENDS+=	tinytemplate-1.0.3
CARGO_CRATE_DEPENDS+=	typenum-1.11.2
CARGO_CRATE_DEPENDS+=	unicode-bidi-0.3.4
CARGO_CRATE_DEPENDS+=	unicode-normalization-0.1.12
CARGO_CRATE_DEPENDS+=	unicode-width-0.1.7
CARGO_CRATE_DEPENDS+=	unicode-xid-0.2.0
CARGO_CRATE_DEPENDS+=	url-2.1.1
CARGO_CRATE_DEPENDS+=	utf-8-0.7.5
CARGO_CRATE_DEPENDS+=	walkdir-2.3.1
CARGO_CRATE_DEPENDS+=	wasi-0.9.0+wasi-snapshot-preview1
CARGO_CRATE_DEPENDS+=	winapi-0.3.8
CARGO_CRATE_DEPENDS+=	winapi-i686-pc-windows-gnu-0.4.0
CARGO_CRATE_DEPENDS+=	winapi-util-0.1.4
CARGO_CRATE_DEPENDS+=	winapi-x86_64-pc-windows-gnu-0.4.0
CARGO_CRATE_DEPENDS+=	xml5ever-0.16.1

BUILDLINK_DEPMETHOD.gobject-introspection+=	build
.include "../../devel/gobject-introspection/buildlink3.mk"
BUILDLINK_API_DEPENDS.glib2+=	glib2>=2.50.0
.include "../../devel/glib2/buildlink3.mk"
BUILDLINK_API_DEPENDS.pango+=	pango>=1.38
.include "../../devel/pango/buildlink3.mk"
.include "../../fonts/fontconfig/buildlink3.mk"
BUILDLINK_API_DEPENDS.cairo+=	cairo>=1.2.0
.include "../../graphics/cairo/buildlink3.mk"
.include "../../graphics/cairo-gobject/buildlink3.mk"
BUILDLINK_API_DEPENDS.freetype2+=	freetype2>=2.8.0
.include "../../graphics/freetype2/buildlink3.mk"
.include "../../graphics/gdk-pixbuf2/loaders.mk"
BUILDLINK_API_DEPENDS.libxml2+=	libxml2>=2.9
.include "../../textproc/libxml2/buildlink3.mk"
.include "../../graphics/gdk-pixbuf2/buildlink3.mk"
RUST_REQ=	1.39.0
.include "../../lang/rust/cargo.mk"
.include "../../mk/bsd.pkg.mk"
