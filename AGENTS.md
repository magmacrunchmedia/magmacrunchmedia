# AGENTS.md

## AI Attribution

**No AI attribution.** Do not append `Co-Authored-By: Claude …`, "Generated with
…", or any similar trailer to commit messages, PR bodies, or release notes. If
your tooling adds such a line by default, remove it before committing.

## This README shares three sections with the org profile

`what we make`, `install` and `source` are duplicated, byte for byte, in
`magmacrunch-media/.github` at `profile/README.md`, which is checked out in this
tree at `web\org-profile`. GitHub profile READMEs cannot include a shared file,
so the only thing keeping them honest is updating both.

Check them with:

```bash
diff <(sed -n '/^<h3 align="left">what we make/,/^For source access/p' README.md) \
     <(sed -n '/^<h3 align="left">what we make/,/^For source access/p' ../org-profile/profile/README.md)
```

The wording is deliberately correct on both pages, which is why the source
section says "the org's repositories" rather than "repositories here": this
account holds one public repository and the org holds the rest.
