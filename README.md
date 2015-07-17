# ncpr
NCPR storage and api

Usage
---

    mkdir -p /opt/data/ncpr

    # build the project
    cargo build

    # load all full data files
    unzip -p {fulldata_file}.zip | ./target/debug/ncpr patch

    # load incremental files in chronological order
    unzip -p {incr_file}.zip | ./target/debug/ncpr patch

    # (optional) run the web server
    node web/app.js
