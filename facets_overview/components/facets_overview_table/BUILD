package(default_visibility = ["//visibility:public"])

load("@org_tensorflow_tensorboard//tensorboard/defs:web.bzl", "ts_web_library")

ts_web_library(
    name = "facets_overview_table",
    srcs = [
        "facets-overview-table.html",
        "facets-overview-table.ts"
    ],
    clutz_entry_points = [
        "proto.featureStatistics.DatasetFeatureStatistics",
        "proto.featureStatistics.DatasetFeatureStatisticsList",
        "proto.featureStatistics.FeatureNameStatistics",
        "proto.featureStatistics.NumericStatistics",
        "proto.featureStatistics.StringStatistics",
        "proto.featureStatistics.CommonStatistics",
        "proto.featureStatistics.Histogram",
        "proto.featureStatistics.RankHistogram"
    ],
    path = "/facets-overview/components/facets-overview-table",
    deps = [
        "//facets_overview/proto",
        "//facets_overview/common",
        "//facets_overview/components/facets_overview_chart",
        "//facets_overview/components/facets_overview_row_legend",
        "//facets_overview/components/facets_overview_row_stats",
        "@org_polymer_iron_list",
        "@org_polymer_paper_dropdown_menu",
        "@org_polymer_paper_item",
        "@org_polymer_paper_listbox",
        "@org_tensorflow_tensorboard//tensorboard/components/tf_imports:d3",
        "@org_tensorflow_tensorboard//tensorboard/components/tf_imports:polymer",
    ],
)

