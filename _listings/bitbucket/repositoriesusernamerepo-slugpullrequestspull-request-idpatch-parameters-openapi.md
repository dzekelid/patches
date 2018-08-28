---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Parameters Repositories Username Repo Slug Pullrequests Pull Request  Patch
  description: Parameters repositories username repo slug pullrequests pull request  patch
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repositories/{username}/{repo_slug}/patch/{spec}:
    get:
      summary: Get Repositories Username Repo Slug Patch Spec
      description: |-
        Produces a raw patch for a single commit (diffed against its first
        parent), or a patch-series for a revspec of 2 commits (e.g.
        `3a8b42..9ff173` where the first commit represents the source and the
        second commit the destination).

        In case of the latter (diffing a revspec), a patch series is returned
        for the commits on the source branch (`3a8b42` and its ancestors in
        our example). For Mercurial, a single patch is returned that combines
        the changes of all commits on the source branch.

        While similar to diffs, patches:

        * Have a commit header (username, commit message, etc)
        * Do not support the `path=foo/bar.py` query parameter

        The raw patch is returned as-is, in whatever encoding the files in the
        repository use. It is not decoded into unicode. As such, the
        content-type is `text/plain`.
      operationId: getRepositoriesUsernameRepoSlugPatchSpec
      x-api-path-slug: repositoriesusernamerepo-slugpatchspec-get
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Patch
      - Spec
    parameters:
      summary: Parameters Repositories Username Repo Slug Patch Spec
      description: Parameters repositories username repo slug patch spec
      operationId: parametersRepositoriesUsernameRepoSlugPatchSpec
      x-api-path-slug: repositoriesusernamerepo-slugpatchspec-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Patch
      - Spec
  /repositories/{username}/{repo_slug}/pullrequests/{pull_request_id}/patch:
    get:
      summary: Get Repositories Username Repo Slug Pullrequests Pull Request  Patch
      description: Get repositories username repo slug pullrequests pull request  patch
      operationId: getRepositoriesUsernameRepoSlugPullrequestsPullRequestPatch
      x-api-path-slug: repositoriesusernamerepo-slugpullrequestspull-request-idpatch-get
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pullrequests
      - Pull
      - Request
      - ""
      - Patch
    parameters:
      summary: Parameters Repositories Username Repo Slug Pullrequests Pull Request  Patch
      description: Parameters repositories username repo slug pullrequests pull request  patch
      operationId: parametersRepositoriesUsernameRepoSlugPullrequestsPullRequestPatch
      x-api-path-slug: repositoriesusernamerepo-slugpullrequestspull-request-idpatch-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pullrequests
      - Pull
      - Request
      - ""
      - Patch
  /snippets/{username}/{encoded_id}/{revision}/patch:
    get:
      summary: Get Snippets Username Encoded  Revision Patch
      description: |-
        Returns the patch of the specified commit against its first
        parent.

        Note that this resource is different in functionality from the `diff`
        resource.

        The differences between a diff and a patch are:

        * patches have a commit header with the username, message, etc
        * diffs support the optional `path=foo/bar.py` query param to filter the
          diff to just that one file diff (not supported for patches)
        * for a merge, the diff will show the diff between the merge commit and
          its first parent (identical to how PRs work), while patch returns a
          response containing separate patches for each commit on the second
          parent's ancestry, up to the oldest common ancestor (identical to
          its reachability).

        Note that the character encoding of the contents of the patch is
        unspecified as Git and Mercurial do not track this, making it hard for
        Bitbucket to reliably determine this.
      operationId: getSnippetsUsernameEncodedRevisionPatch
      x-api-path-slug: snippetsusernameencoded-idrevisionpatch-get
      parameters:
      - in: path
        name: encoded_id
        description: The snippet id
      - in: path
        name: revision
        description: A revspec expression
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Revision
      - Patch
    parameters:
      summary: Parameters Snippets Username Encoded  Revision Patch
      description: Parameters snippets username encoded  revision patch
      operationId: parametersSnippetsUsernameEncodedRevisionPatch
      x-api-path-slug: snippetsusernameencoded-idrevisionpatch-parameters
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Revision
      - Patch
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---