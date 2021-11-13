# 0005 - "update" API endpoint

Date: Nov 10, 2021

## Context

The application needs to support the handle update operation needed by Avalon.

Avalon needs to be able to update an existing Fedora 2 handle to change the handle
resolution URL and metadata to reflect the migration into Avalon. The handle to
be updated will be identfied using:

* "prefix" and "suffix"

If a handle exists, the following information can be updated:

* repo
* repo_id
* url
* description
* notes

## Decision

It was decided to implement the functionality needed by Avalon using the
/handle/prefix/suffix endpoint with PATCH method.

## Consequences

Handles can now by updated via the JSON API.
