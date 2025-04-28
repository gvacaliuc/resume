# gabriel vacaliuc

I like building things and playing ultimate

contact:  
* https://github.com/gvacaliuc
* gabe.vacaliuc@gmail.com
* https://www.linkedin.com/in/gabriel-vacaliuc-7aa698131
* (865) 410-8388

## languages / skills

* languages: go,python,scala,java,bash,typescript
* tools/frameworks: kafka,bazel,spark,linux,python data stack,docker,k8s
* skills: shipping quickly,reviewing code,improving others code

## work experience

### Included Health (Aug. '20 - now)

I am part of a 3 person engineer only team responsible for our core data
infrastructure.  This includes a spark-on-k8s based batch platform,
frontend/backend eventing libraries, and more recently a golang protobuf-based
document store library with transactional eventing.

Our batch data platform is used by ~30 teams and regularly processes ~40TB of
data per day.  Since I've joined the reliability of the platform has improved
from approximately one downtime event per week to less than one per year.

In the past 2 years, we've been focusing on building out our real-time data
platform on top of kafka.  Outside of core platform work making it easy to
produce / consume from kafka, recent large projects include leading a team to
unify our model of "users" from 3 legacy systems into one and making it easy to
use real-time data in online inference in our nascent ML Platform.

### Cruise (summer '19)

I interned on the developer platform team and improved C++ build times.

* collected all bazel profile data into BQ
* basic looker / datastudio dashboards measuring build critical path and slowest packages
* linter to identify template classes / functions which balloon # of concrete compilation targets
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

### Oak Ridge National Laboratory (summer '14 - summer '16)

I spent about 2.5y during high school at https://ornl.gov as a student
researcher under Arvind Ramanathan.  I learned a lot about ML and Linux.
