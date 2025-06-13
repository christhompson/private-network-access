
# Private Network Access

**Note: Private Network Access is [on hold](https://developer.chrome.com/blog/pna-on-hold). Work is currently continuing on a new proposal to gate local network access behind a permission – see the [Local Network Access explainer](https://github.com/explainers-by-googlers/local-network-access) and [Chrome's blog post with details for developers](https://developer.chrome.com/blog/local-network-access).**

This is the repository for the Private Network Access specification (initially known as *CORS-RFC1918*).

You may be interested in reading:

 - the specification: https://wicg.github.io/private-network-access/
 - the explainer:
   [`./explainer.md`](https://github.com/WICG/private-network-access/blob/master/explainer.md)
 - the security & privacy self-review:
   [`./security_privacy_self_review.md`](https://github.com/WICG/private-network-access/blob/master/security_privacy_self_review.md)

 - Permission prompt:
   - the explainer:
   [`./permission_prompt/explainer.md`](https://github.com/WICG/private-network-access/blob/master/permission_prompt/explainer.md)
   - the security & privacy self-review:
   [`./permission_prompt/security_privacy_self_review.md`](https://github.com/WICG/private-network-access/blob/master/permission_prompt/security_privacy_self_review.md)

## How to build

Ensure you have [pipenv](https://github.com/pypa/pipenv) installed, then:

```sh
$ make
```

While this is useful when editing the spec locally, do not commit the generated
HTML file to the `main` branch. That is taken care of automatically upon pushing
to `main` by a github workflow.

## How to deploy

`index.src.html` is automatically built with
[bikeshed](https://github.com/speced/bikeshed) and published to the `gh-pages`
branch using the [spec-prod](https://github.com/w3c/spec-prod) action.
