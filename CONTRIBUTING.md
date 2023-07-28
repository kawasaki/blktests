# Contributing to blktests

You can contribute to blktests by sending patches to the
<linux-block@vger.kernel.org> mailing list and Shin'ichiro Kawasaki <shinichiro.kawasaki@wdc.com>
or by opening a pull request to the [blktests GitHub
repository](https://github.com/osandov/blktests). Patch post is more recommended
since it will be visible to more kernel developers and easier to gather
feedback. If sending patches, please generate the patch with `git format-patch
--subject-prefix="PATCH blktests"`. Consider configuring git to do this for you
with `git config --local format.subjectPrefix "PATCH blktests"`.

All commits must be signed off (i.e., `Signed-off-by: Jane Doe <janedoe@example.org>`)
as per the [Developer Certificate of Origin](https://developercertificate.org/).
`git commit -s` and `git format-patch -s` can do this for you.

Please run `make check` before submitting a new test. This runs the
[shellcheck](https://github.com/koalaman/shellcheck) static analysis tool and
some other sanity checks.
