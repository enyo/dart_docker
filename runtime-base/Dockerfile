# Copyright (c) 2014, the Dart project authors.  Please see the AUTHORS file
# for details. All rights reserved. Use of this source code is governed by a
# BSD-style license that can be found in the LICENSE file.
#
# Dockerfile for google/dart-runtime-base

FROM google/dart

ADD dart_run.sh /dart_runtime/
RUN chmod 755 /dart_runtime/dart_run.sh && \
  chown root:root /dart_runtime/dart_run.sh

# Expose ports for debugger (5858), application traffic (8080)
# and the observatory (8181)
EXPOSE 8080 8181 5858

CMD []
ENTRYPOINT ["/dart_runtime/dart_run.sh"]
