---
name: Bitbucket
x-slug: bitbucket
description: Collaborate on code with inline comments and pull requests. Manage and
  share your Git repositories to build and ship software, as a team.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
x-kinRank: "8"
x-alexaRank: "901"
tags: Commits
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/apis.md
specificationVersion: "0.14"
apis:
- name: Bitbucket - Get Repositories Username Repo Slug Commits
  x-api-slug: repositoriesusernamerepo-slugcommits-get
  description: |-
    These are the repository's commits. They are paginated and returned
    in reverse chronological order, similar to the output of `git log` and
    `hg log`. Like these tools, the DAG can be filtered.

    ## GET /repositories/{username}/{repo_slug}/commits/

    Returns all commits in the repo in topological order (newest commit
    first). All branches and tags are included (similar to
    `git log --all` and `hg log`).

    ## GET /repositories/{username}/{repo_slug}/commits/master

    Returns all commits on rev `master` (similar to `git log master`,
    `hg log master`).

    ## GET /repositories/{username}/{repo_slug}/commits/dev?exclude=master

    Returns all commits on ref `dev`, except those that are reachable on
    `master` (similar to `git log dev ^master`).

    ## GET /repositories/{username}/{repo_slug}/commits/?exclude=master

    Returns all commits in the repo that are not on master
    (similar to `git log --all ^master`).

    ## GET /repositories/{username}/{repo_slug}/commits/?include=foo&include=bar&exclude=fu&exclude=fubar

    Returns all commits that are on refs `foo` or `bar`, but not on `fu` or
    `fubar` (similar to `git log foo bar ^fu ^fubar`).

    Because the response could include a very large number of commits, it
    is paginated. Follow the 'next' link in the response to navigate to the
    next page of commits. As with other paginated resources, do not
    construct your own links.

    When the include and exclude parameters are more than can fit in a
    query string, clients can use a `x-www-form-urlencoded` POST instead.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommits-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommits-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commits
  x-api-slug: repositoriesusernamerepo-slugcommits-parameters
  description: Parameters repositories username repo slug commits
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommits-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommits-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Commits
  x-api-slug: repositoriesusernamerepo-slugcommits-post
  description: |-
    Identical to `GET /repositories/{username}/{repo_slug}/commits`,
    except that POST allows clients to place the include and exclude
    parameters in the request body to avoid URL length issues.

    **Note that this resource does NOT support new commit creation.**
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommits-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommits-post-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commits Revision
  x-api-slug: repositoriesusernamerepo-slugcommitsrevision-get
  description: |-
    These are the repository's commits. They are paginated and returned
    in reverse chronological order, similar to the output of `git log` and
    `hg log`. Like these tools, the DAG can be filtered.

    ## GET /repositories/{username}/{repo_slug}/commits/

    Returns all commits in the repo in topological order (newest commit
    first). All branches and tags are included (similar to
    `git log --all` and `hg log`).

    ## GET /repositories/{username}/{repo_slug}/commits/master

    Returns all commits on rev `master` (similar to `git log master`,
    `hg log master`).

    ## GET /repositories/{username}/{repo_slug}/commits/dev?exclude=master

    Returns all commits on ref `dev`, except those that are reachable on
    `master` (similar to `git log dev ^master`).

    ## GET /repositories/{username}/{repo_slug}/commits/?exclude=master

    Returns all commits in the repo that are not on master
    (similar to `git log --all ^master`).

    ## GET /repositories/{username}/{repo_slug}/commits/?include=foo&include=bar&exclude=fu&exclude=fubar

    Returns all commits that are on refs `foo` or `bar`, but not on `fu` or
    `fubar` (similar to `git log foo bar ^fu ^fubar`).

    Because the response could include a very large number of commits, it
    is paginated. Follow the 'next' link in the response to navigate to the
    next page of commits. As with other paginated resources, do not
    construct your own links.

    When the include and exclude parameters are more than can fit in a
    query string, clients can use a `x-www-form-urlencoded` POST instead.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commits Revision
  x-api-slug: repositoriesusernamerepo-slugcommitsrevision-parameters
  description: Parameters repositories username repo slug commits revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Commits Revision
  x-api-slug: repositoriesusernamerepo-slugcommitsrevision-post
  description: |-
    Identical to `GET /repositories/{username}/{repo_slug}/commits`,
    except that POST allows clients to place the include and exclude
    parameters in the request body to avoid URL length issues.

    **Note that this resource does NOT support new commit creation.**
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-post-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pullrequests Pull Request  Commits
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-idcommits-get
  description: |-
    Returns a paginated list of the pull request's commits.

    These are the commits that are being merged into the destination
    branch when the pull requests gets accepted.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcommits-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcommits-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Pullrequests Pull Request  Commits
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-idcommits-parameters
  description: Parameters repositories username repo slug pullrequests pull request  commits
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcommits-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcommits-parameters-openapi.md
- name: Bitbucket - Get Snippets Username Encoded  Commits
  x-api-slug: snippetsusernameencoded-idcommits-get
  description: Returns the changes (commits) made on this snippet.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/snippetsusernameencoded-idcommits-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/snippetsusernameencoded-idcommits-get-openapi.md
- name: Bitbucket - Parameters Snippets Username Encoded  Commits
  x-api-slug: snippetsusernameencoded-idcommits-parameters
  description: Parameters snippets username encoded  commits
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/snippetsusernameencoded-idcommits-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/snippetsusernameencoded-idcommits-parameters-openapi.md
- name: Bitbucket - Get Snippets Username Encoded  Commits Revision
  x-api-slug: snippetsusernameencoded-idcommitsrevision-get
  description: Get snippets username encoded  commits revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/snippetsusernameencoded-idcommitsrevision-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/snippetsusernameencoded-idcommitsrevision-get-openapi.md
- name: Bitbucket - Parameters Snippets Username Encoded  Commits Revision
  x-api-slug: snippetsusernameencoded-idcommitsrevision-parameters
  description: Parameters snippets username encoded  commits revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/snippetsusernameencoded-idcommitsrevision-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/snippetsusernameencoded-idcommitsrevision-parameters-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Commit Node Approve
  x-api-slug: repositoriesusernamerepo-slugcommitnodeapprove-delete
  description: |-
    Redact the authenticated user's approval of the specified commit.

    This operation is only available to users that have explicit access to
    the repository. In contrast, just the fact that a repository is
    publicly accessible to users does not give them the ability to approve
    commits.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodeapprove-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodeapprove-delete-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Node Approve
  x-api-slug: repositoriesusernamerepo-slugcommitnodeapprove-parameters
  description: Parameters repositories username repo slug commit node approve
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodeapprove-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodeapprove-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Commit Node Approve
  x-api-slug: repositoriesusernamerepo-slugcommitnodeapprove-post
  description: |-
    Approve the specified commit as the authenticated user.

    This operation is only available to users that have explicit access to
    the repository. In contrast, just the fact that a repository is
    publicly accessible to users does not give them the ability to approve
    commits.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodeapprove-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodeapprove-post-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commit Node Statuses
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatuses-get
  description: Returns all statuses (e.g. build results) for a specific commit.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatuses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatuses-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Node Statuses
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatuses-parameters
  description: Parameters repositories username repo slug commit node statuses
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatuses-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatuses-parameters-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Node Statuses
    Build
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatusesbuild-parameters
  description: Parameters repositories username repo slug commit node statuses build
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuild-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuild-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Commit Node Statuses Build
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatusesbuild-post
  description: |-
    Creates a new build status against the specified commit.

    If the specified key already exists, the existing status object will
    be overwritten.

    When creating a new commit status, you can use a URI template for the URL.
    Templates are URLs that contain variable names that Bitbucket will
    evaluate at runtime whenever the URL is displayed anywhere similar to
    parameter substitution in
    [Bitbucket Connect](https://developer.atlassian.com/bitbucket/concepts/context-parameters.html).
    For example, one could use `https://foo.com/builds/{repository.full_name}`
    which Bitbucket will turn into `https://foo.com/builds/foo/bar` at render time.
    The context variables available are `repository` and `commit`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuild-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuild-post-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commit Node Statuses Build
    Key
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatusesbuildkey-get
  description: Get repositories username repo slug commit node statuses build key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Node Statuses
    Build Key
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatusesbuildkey-parameters
  description: Parameters repositories username repo slug commit node statuses build
    key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-parameters-openapi.md
- name: Bitbucket - Update Repositories Username Repo Slug Commit Node Statuses Build
    Key
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatusesbuildkey-put
  description: |-
    Used to update the current status of a build status object on the
    specific commit.

    This operation can also be used to change other properties of the
    build status:

    * `state`
    * `name`
    * `description`
    * `url`
    * `refname`

    The `key` cannot be changed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-put-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commit Revision
  x-api-slug: repositoriesusernamerepo-slugcommitrevision-get
  description: Get repositories username repo slug commit revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Revision
  x-api-slug: repositoriesusernamerepo-slugcommitrevision-parameters
  description: Parameters repositories username repo slug commit revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commit Sha Comments
  x-api-slug: repositoriesusernamerepo-slugcommitshacomments-get
  description: |-
    Returns the commit's comments.

    This includes both global and inline comments.

    The default sorting is oldest to newest and can be overridden with
    the `sort` query parameter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacomments-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Sha Comments
  x-api-slug: repositoriesusernamerepo-slugcommitshacomments-parameters
  description: Parameters repositories username repo slug commit sha comments
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacomments-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacomments-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commit Sha Comments Comment
  x-api-slug: repositoriesusernamerepo-slugcommitshacommentscomment-id-get
  description: Get repositories username repo slug commit sha comments comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacommentscomment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacommentscomment-id-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Sha Comments
    Comment
  x-api-slug: repositoriesusernamerepo-slugcommitshacommentscomment-id-parameters
  description: Parameters repositories username repo slug commit sha comments comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacommentscomment-id-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacommentscomment-id-parameters-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Sha Comments
    Comment
  x-api-slug: repositoriesusernamerepo-slugcommitshacommentscomment-id-parameters
  description: Parameters repositories username repo slug commit sha comments comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacommentscomment-id-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacommentscomment-id-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commit Sha Comments Comment
  x-api-slug: repositoriesusernamerepo-slugcommitshacommentscomment-id-get
  description: Get repositories username repo slug commit sha comments comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacommentscomment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacommentscomment-id-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Sha Comments
  x-api-slug: repositoriesusernamerepo-slugcommitshacomments-parameters
  description: Parameters repositories username repo slug commit sha comments
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacomments-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacomments-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commit Sha Comments
  x-api-slug: repositoriesusernamerepo-slugcommitshacomments-get
  description: |-
    Returns the commit's comments.

    This includes both global and inline comments.

    The default sorting is oldest to newest and can be overridden with
    the `sort` query parameter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacomments-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Revision
  x-api-slug: repositoriesusernamerepo-slugcommitrevision-parameters
  description: Parameters repositories username repo slug commit revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commit Revision
  x-api-slug: repositoriesusernamerepo-slugcommitrevision-get
  description: Get repositories username repo slug commit revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-get-openapi.md
- name: Bitbucket - Update Repositories Username Repo Slug Commit Node Statuses Build
    Key
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatusesbuildkey-put
  description: |-
    Used to update the current status of a build status object on the
    specific commit.

    This operation can also be used to change other properties of the
    build status:

    * `state`
    * `name`
    * `description`
    * `url`
    * `refname`

    The `key` cannot be changed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-put-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Node Statuses
    Build Key
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatusesbuildkey-parameters
  description: Parameters repositories username repo slug commit node statuses build
    key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commit Node Statuses Build
    Key
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatusesbuildkey-get
  description: Get repositories username repo slug commit node statuses build key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-get-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Commit Node Statuses Build
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatusesbuild-post
  description: |-
    Creates a new build status against the specified commit.

    If the specified key already exists, the existing status object will
    be overwritten.

    When creating a new commit status, you can use a URI template for the URL.
    Templates are URLs that contain variable names that Bitbucket will
    evaluate at runtime whenever the URL is displayed anywhere similar to
    parameter substitution in
    [Bitbucket Connect](https://developer.atlassian.com/bitbucket/concepts/context-parameters.html).
    For example, one could use `https://foo.com/builds/{repository.full_name}`
    which Bitbucket will turn into `https://foo.com/builds/foo/bar` at render time.
    The context variables available are `repository` and `commit`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuild-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuild-post-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Node Statuses
    Build
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatusesbuild-parameters
  description: Parameters repositories username repo slug commit node statuses build
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuild-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuild-parameters-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Node Statuses
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatuses-parameters
  description: Parameters repositories username repo slug commit node statuses
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatuses-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatuses-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commit Node Statuses
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatuses-get
  description: Returns all statuses (e.g. build results) for a specific commit.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatuses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatuses-get-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Commit Node Approve
  x-api-slug: repositoriesusernamerepo-slugcommitnodeapprove-post
  description: |-
    Approve the specified commit as the authenticated user.

    This operation is only available to users that have explicit access to
    the repository. In contrast, just the fact that a repository is
    publicly accessible to users does not give them the ability to approve
    commits.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodeapprove-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodeapprove-post-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Node Approve
  x-api-slug: repositoriesusernamerepo-slugcommitnodeapprove-parameters
  description: Parameters repositories username repo slug commit node approve
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodeapprove-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodeapprove-parameters-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Commit Node Approve
  x-api-slug: repositoriesusernamerepo-slugcommitnodeapprove-delete
  description: |-
    Redact the authenticated user's approval of the specified commit.

    This operation is only available to users that have explicit access to
    the repository. In contrast, just the fact that a repository is
    publicly accessible to users does not give them the ability to approve
    commits.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodeapprove-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commits/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodeapprove-delete-openapi.md
x-common:
- type: x-api-gallery
  url: http://bigoven.api.gallery.streamdata.io
- type: x-api-stack
  url: http://bitbucket.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/bitbucket
- type: x-developer
  url: https://developer.atlassian.com/cloud/bitbucket/
- type: x-documentation
  url: https://confluence.atlassian.com/bitbucket/bitbucket-cloud-documentation-221448814.html?_ga=2.77295890.629375793.1519179030-1077111323.1516485126
- type: x-status
  url: https://status.bitbucket.org/?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-support
  url: https://support.atlassian.com/bitbucket-cloud/
- type: x-terms-of-service
  url: https://www.atlassian.com/legal/customer-agreement?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-twitter
  url: https://twitter.com/bitbucket
- type: x-website
  url: http://bitbucket.org
- type: x-website
  url: https://bitbucket.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---