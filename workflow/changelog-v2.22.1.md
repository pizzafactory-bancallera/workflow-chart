
#### Releases

- builder v2.13.6 -> v2.13.7
- controller v2.21.0 -> v2.21.1
- dockerbuilder v2.8.2 -> v2.8.3
- minio v2.4.4 -> v2.4.5
- postgres v2.7.4 -> v2.7.5
- redis v2.4.1 -> v2.4.2
- registry v2.6.0 -> v2.6.1
- registry-proxy v1.5.0 -> v1.5.1
- registry-token-refresher v1.2.1 -> v1.2.2
- router v2.18.0 -> v2.18.1
- slugbuilder v2.7.6 -> v2.7.7
- slugrunner v2.6.2 -> v2.6.3
- workflow v2.22.0 -> v2.22.1
- workflow-cli v2.22.0 -> v2.22.1
- workflow-e2e v2.22.0 -> v2.22.1

#### Features

- [`7c59d1c`](https://github.com/teamhephy/controller/commit/7c59d1cda80a606be8fd67b1021a3d56347f13d4) (controller) - controller/logging: Add flag to enable verbose logging
- [`951c8ba`](https://github.com/teamhephy/registry-proxy/commit/951c8ba6d31abafcfcc4e516d25e93ac048ab31c) (registry-proxy) - nginx: upgrade nginx to 1.18

#### Refactors

- [`819bebf`](https://github.com/teamhephy/postgres/commit/819bebfc340a9d1370df482b93529cdcf8b217b0) (postgres) - Dockerfile: upgrade dockerfile packages for postgres
- [`bcaab90`](https://github.com/teamhephy/postgres/commit/bcaab9097c57422cca182d0d57202f375bdf52a1) (postgres) - azure: start using new azure storage BlobServiceClient
- [`a848e8e`](https://github.com/teamhephy/registry-token-refresher/commit/a848e8e321da1477cc492aaaa589421ad0713040) (registry-token-refresher) - golang: rename this repo inside self everywhere

#### Fixes

- [`9c66b39`](https://github.com/teamhephy/controller/commit/9c66b3924326f108c45d8adc7ef110fac177cfb0) (controller) - charts: controller needs the "patch" perm
- [`bb05432`](https://github.com/teamhephy/controller/commit/bb05432f004644b8cdd584affbbb3664771d0afc) (controller) - controller: adding scale_api_version to Scale
- [`d43b5fa`](https://github.com/teamhephy/controller/commit/d43b5fa7d58335328808c22a961da439e2dde045) (controller) - controller: apps/v1 in App model for hpa
- [`f0579e0`](https://github.com/teamhephy/redis/commit/f0579e0ce7b5141636deeb79512ab80dbe4f3336) (redis) - style: fix style per shellcheck
- [`f46527e`](https://github.com/teamhephy/slugbuilder/commit/f46527e39eda6ae68df37f7340e658eb41574f3c) (slugbuilder) - build.sh: fix shellcheck failures and warnings
- [`793ab0a`](https://github.com/teamhephy/slugbuilder/commit/793ab0ac11c6054d84f996f0eb08fae6332f8f30) (slugbuilder) - Makefile: change image prefix to hephy
- [`3035c6e`](https://github.com/teamhephy/workflow/commit/3035c6ec7342f2c77b989d532640e7940b8938c1) (workflow) - charts: allow "" for Values.s3.accesskey|secretkey for helm3

#### Documentation

- [`fb9bd29`](https://github.com/teamhephy/registry-proxy/commit/fb9bd2997018e582b22b38982ccb4d73a740a27c) (registry-proxy) - README: update the annoucement in repo

#### Maintenance

- [`f0058e5`](https://github.com/teamhephy/builder/commit/f0058e59f8f3917c40364514176af3385fd9c5b4) (builder) - Makefile: chore(Makefile) upgrading go-dev container to v1.28.3
- [`488d8b0`](https://github.com/teamhephy/dockerbuilder/commit/488d8b09aef5af34da162fca0ca50fd69bb1cab0) (dockerbuilder) - dockerrunner: storage cli
- [`586c181`](https://github.com/teamhephy/dockerbuilder/commit/586c181a2cce46acd6757ddfc721073d742827c8) (dockerbuilder) - slugbuilder: use better tested binary
- [`7caf660`](https://github.com/teamhephy/minio/commit/7caf660c3c69286a437c66df232209e1b0313ceb) (minio) - Makefile: upgrading go-dev container to v1.28.3
- [`acdf534`](https://github.com/teamhephy/minio/commit/acdf5349b681b56ba31d3acc1f46a8a33dd3ddb5) (minio) - minio: upgrading pkg package and some renaming
- [`66f3268`](https://github.com/teamhephy/postgres/commit/66f326853b54461db654cdcf20760c355940b63d) (postgres) - Makefile: upgrading go-dev container to v1.28.3
- [`70d2867`](https://github.com/teamhephy/redis/commit/70d2867c1b21d2c6d1708efa3a65a0f597c255d7) (redis) - Makefile: upgrading go-dev container to v1.28.3
- [`570da3e`](https://github.com/teamhephy/registry/commit/570da3e4a42015de6ceb638760491d694a96bd41) (registry) - Makefile: upgrading go-dev container to v1.28.3
- [`b6fe20b`](https://github.com/teamhephy/registry/commit/b6fe20b74e6677ea15a999b1b4281a75a2572dff) (registry) - registry: rename a few necessary things
- [`ed8e945`](https://github.com/teamhephy/registry-proxy/commit/ed8e9458a90c389ba49b4738f1f6a666820ccc29) (registry-proxy) - registry-proxy: permit umbrella override api group
- [`bca00d4`](https://github.com/teamhephy/registry-proxy/commit/bca00d48338c9738cdced9a6df75021ccc9a4952) (registry-proxy) - charts: define APIVersion template
- [`4e597fc`](https://github.com/teamhephy/registry-proxy/commit/4e597fc7338f7c77650cd4430d39dbdbf2e31739) (registry-proxy) - charts: switch to hephy docker hub org
- [`303cea3`](https://github.com/teamhephy/registry-proxy/commit/303cea3a8f0d3a5b534c2f31ef0bfe241adcdc61) (registry-proxy) - charts: remove quay.io from ds
- [`13fe498`](https://github.com/teamhephy/registry-token-refresher/commit/13fe498d68d6e49fa1f1547e6fc755e1f16ffa1b) (registry-token-refresher) - Makefile: upgrading go-dev container to v1.28.3
- [`9c7375a`](https://github.com/teamhephy/registry-token-refresher/commit/9c7375a4cd68b00e4bf7347ff01b00e5892171bc) (registry-token-refresher) - rootfs: use hephy/base:v0.4.1 base image
- [`282d800`](https://github.com/teamhephy/registry-token-refresher/commit/282d800631849fda90e7f0cbad6992b8053ed79f) (registry-token-refresher) - glide: update/remove some golang packages
- [`735d905`](https://github.com/teamhephy/router/commit/735d90548e52f0755ba4582d033f6c3a27d98000) (router) - Makefile: v1.28.3 image
- [`a8832b8`](https://github.com/teamhephy/slugbuilder/commit/a8832b84f3924a574efd76cfcf7c1e3ec41f108c) (slugbuilder) - slugbuilder: revert 41fc96af in Dockerfile
- [`0aaaf09`](https://github.com/teamhephy/slugbuilder/commit/0aaaf09405197fc752eecbec943ef4f98da15e6e) (slugbuilder) - slugbuilder: new build, new objstorage
- [`e90960d`](https://github.com/teamhephy/slugbuilder/commit/e90960d75ecfeb54074dcffff9bd98df8770f602) (slugbuilder) - buildpacks: update all buildpacks to latest versions
- [`d7570c4`](https://github.com/teamhephy/slugbuilder/commit/d7570c4b9a48800bc61398fce54d6490c77be23c) (slugbuilder) - slugbuilder: use better tested binary
- [`4931bfd`](https://github.com/teamhephy/slugbuilder/commit/4931bfd1f6b2eec74a802522ceb675d83afe008f) (slugbuilder) - Makefile: chore(Makefile) upgrading go-dev container to v1.28.3
- [`37d0709`](https://github.com/teamhephy/slugrunner/commit/37d070964c9e3333f3effc6db56d320910e7a157) (slugrunner) - slugrunner: rebuild slugrunner, objstorage
- [`cc52ab2`](https://github.com/teamhephy/slugrunner/commit/cc52ab23e24fe034640662b4815bdfc6aa5fa8e7) (slugrunner) - slugrunner: peg objstorage to the last known good version
- [`968deb5`](https://github.com/teamhephy/slugrunner/commit/968deb5ae2685afb35013940c59f308059923265) (slugrunner) - Makefile: chore(Makefile) upgrading go-dev container to v1.28.3
- [`07c9bc5`](https://github.com/teamhephy/workflow/commit/07c9bc5b0b2ab378ae2104b328ecaf536b6b55d8) (workflow) - charts: add AZURE_STORAGE_CONNECTION_STRING to values.yaml
