# Versioning

All versioning will follow a <major>.<minor>.<patch>.[<pre-release>] style

- Major
    Indicates a breaking change in the public API.  If the expected behavior changes in a manner  
    that breaks previous requests that would have succeeded then the major version will  
    be bumped.  Note that bug fixes may result in practical changes to the API.  However,  
    these are not considered changes to the expected behavior and therefore do not necessarily  
    constitute major changes.
- Minor
    Any change in the public API that is completely backwards compatible.  All previous  
    usages will still work, however there may be new/extended capabilities  
    that were not previously available.  Typically used for feature enhancements
- Patch
    Any change that does not impact the expected behavior of the public API.  This typically  
    include bug fixes and performance enhancements.  Note that certain bug fixes may require  
    a practical change in the API.  For example if there was a function that was called `multiply`  
    but it was actually adding the inputs, despite this technically changing the inputs, the  
    expected behavior has not changes and therefore fixing this bug would be considered a patch.
- Pre-Release
    An arbitrary suffix that indicates that the release is not necessarily production ready.  
    The suffix must begin with a letter such as `rc2` or `b1`.
    
## Pre-1.0.0 Releases

Any version before `1.0.0` is considered unstable.  There may be breaking changes
between any version less than `1.0.0`

## tl;dr

You can safely fix your version to the desired `Major` version without worrying  
about changes to the minor and patch versions.  If it currently works on 1.2.3 it should  
work on all versions < 2.0.0.  The one caveat is that versions < 1.0.0 are considered unstable  
and you should fix them to the exact version you need.
