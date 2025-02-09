# gabriel vacaliuc

I like building things and playing ultimate

contact:  
* https://github.com/gvacaliuc
* gabe.vacaliuc@gmail.com
* https://www.linkedin.com/in/gabriel-vacaliuc-7aa698131
* (865) 410-8388

## languages / skills

* languages: go,scala,python,java,bash,typescript
* tools/frameworks: bazel,spark,linux,python data stuff,docker,jupyterhub
* skills: shipping quickly,reviewing code,improving others code

## work experience

### Included Health (Aug. '20 - now)

I am part of a 3 person engineer only team responsible for our core data
infrastructure.  This includes a spark-on-k8s based batch platform,
frontend/backend eventing libraries, and more recently a golang protobuf-based
document store library with transactional eventing.

Our batch data platform is used by ~30 teams and regularly processes ~40TB of
data per day.  Since I've joined the reliability of the platform has improved
from approximately one downtime event per week to a handful in the past year.

More recently, we have been focusing efforts "upstream" on the backend services
producing and using data in order to shift the primary source of data from
nightly database snapshots to real-time events.

In the past few months, I embedded with a backend team building on these core
service primitives and expanding them as needed.  I led the team in unifying our
model of "users" from 3 legacy systems into one, unblocking deprecating the remaining pieces.

Presently I'm focused on improving developer tooling for our data services
and making it easy to use real-time data for online inference in our nascent
ML Platform.

### Cruise (summer '19)

I interned on the developer platform team working on improving C++ build times.

* collected all bazel profile data into BQ
* basic looker / datastudio dashboards measuring build critical path and slowest packages
* tool to identify classes / functions which unnecessarily balloon # of concrete compilation targets
* reduced build critical path by ~25%

### Two Sigma (summer '17/'18)

I interned at TS for two summers.

* first year (after freshman year of college)
    * implemented some pandas data pipelines to calculate margin requirements
* second year: https://youtu.be/rQd9Zd1ONOw
    * implemented xattr support in internal fuse virtual filesystem
    * exposed precomputed file digests via xattrs
    * forked bazel to use file digests instead of transferring files for file hashes
    * goal was to decrease incremental build times when files don't change (using precomputed digest is cheaper than downloading and hashing file)
    * didn't work
        * variance in build time decreased dramatically
        * overall build time remained relatively constant
