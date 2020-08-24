# playground for download-artifact [issue#42]

@benjamincharity wrote in [issue#42] of action "download-artifact"
> ... from what I've seen each method will still mark our workflow as failed in the PR and primary repo badge. So any contributor or consumer needs to actually go see if our build is really failing or if it is just one optional step that is failing.
Source: https://github.com/actions/download-artifact/issues/42#issuecomment-679076117

This repo was made to see if this is true.

---

conclusion: @benjamincharity was wrong

This means `continue-on-error: true` should work for him.

As expected
* the repo's action status is a green checkmark
* al actions pass, regardless of the failing step

[issue#42]: https://github.com/actions/download-artifact/issues/42
