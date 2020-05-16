# Changelog

##### Version 3.18 and later

Changelog moved to [GitHub Releases](https://github.com/jenkinsci/swarm-plugin/releases).

##### Version 3.17 (June 2, 2019)

-   Swarm plugin
    -   Add integration test framework
        ([\#81](https://github.com/jenkinsci/swarm-plugin/pull/81))
    -   Add test for
        [JENKINS-39443](https://issues.jenkins-ci.org/browse/JENKINS-39443)
        ([\#100](https://github.com/jenkinsci/swarm-plugin/pull/100))
    -   Miscellaneous code cleanup
        ([\#86](https://github.com/jenkinsci/swarm-plugin/pull/86),
        [\#91](https://github.com/jenkinsci/swarm-plugin/pull/91),
        [\#92](https://github.com/jenkinsci/swarm-plugin/pull/92),
        [\#93](https://github.com/jenkinsci/swarm-plugin/pull/93),
        [\#94](https://github.com/jenkinsci/swarm-plugin/pull/94),
        [\#97](https://github.com/jenkinsci/swarm-plugin/pull/97),
        [\#101](https://github.com/jenkinsci/swarm-plugin/pull/101),
        [\#108](https://github.com/jenkinsci/swarm-plugin/pull/108),
        [\#109](https://github.com/jenkinsci/swarm-plugin/pull/109))
-   Swarm client
    -   Fix
        [SECURITY-1252](https://jenkins.io/security/advisory/2019-04-30/#SECURITY-1252)
        XML External Entity (XXE) vulnerability
        ([\#84](https://github.com/jenkinsci/swarm-plugin/pull/84),
        [\#90](https://github.com/jenkinsci/swarm-plugin/pull/90),
        [\#96](https://github.com/jenkinsci/swarm-plugin/pull/96))
    -   Rework logging of command-line arguments
        ([\#95](https://github.com/jenkinsci/swarm-plugin/pull/95))
    -   Fix
        [JENKINS-42930](https://issues.jenkins-ci.org/browse/JENKINS-42930) Use
        System proxy when available and migrate from [Commons HttpClient
        3.x](https://hc.apache.org/httpclient-3.x/) to
        [HttpComponents Client
        4.x](https://hc.apache.org/httpcomponents-client-ga/index.html)
        ([\#105](https://github.com/jenkinsci/swarm-plugin/pull/105),
        [Documentation](docs/proxy.md))
    -   Fix
        [JENKINS-45295](https://issues.jenkins-ci.org/browse/JENKINS-45295)
        Swarm client should update labels on the fly when labels file
        changes
        ([\#104](https://github.com/jenkinsci/swarm-plugin/pull/104),
        [\#110](https://github.com/jenkinsci/swarm-plugin/pull/110))
    -   Fix
        [JENKINS-50970](https://issues.jenkins-ci.org/browse/JENKINS-50970)
        SLF4J logging not working in Swarm client
        ([\#98](https://github.com/jenkinsci/swarm-plugin/pull/98),
        [\#99](https://github.com/jenkinsci/swarm-plugin/pull/99),
        [\#102](https://github.com/jenkinsci/swarm-plugin/pull/102),
        [\#106](https://github.com/jenkinsci/swarm-plugin/pull/106),
        [Documentation](docs/logging.md))
    -   Fix invalid exit code
        ([\#103](https://github.com/jenkinsci/swarm-plugin/pull/103))
    -   Remove deprecated `-logFile` parameter
        ([\#107](https://github.com/jenkinsci/swarm-plugin/pull/107))

##### Version 3.16 (May 21, 2019)

-   Swarm plugin
    -   Update minimum Jenkins core requirement to 2.60.3
        ([\#87](https://github.com/jenkinsci/swarm-plugin/pull/87))
    -   Remove unnecessary field
        ([\#85](https://github.com/jenkinsci/swarm-plugin/pull/85))
-   Swarm client
    -   Disable DTDs completely in all XML parsers to prevent XML
        External Entity (XXE) attacks
        ([\#84](https://github.com/jenkinsci/swarm-plugin/pull/84))
    -   Update Jenkins Remoting version from 3.28 to 3.30
        ([\#78](https://github.com/jenkinsci/swarm-plugin/pull/78),
        [full
        changelog](https://github.com/jenkinsci/remoting/blob/master/CHANGELOG.md))

##### Version 3.15 (December 12, 2018)

-   Swarm plugin
    -   Fix the label removal in the `removeLabels` endpoint
        ([\#75](https://github.com/jenkinsci/swarm-plugin/pull/75))
-   Swarm client
    -   Update Jenkins Remoting version from 3.26 to 3.28 to pick up new
        stability fixes ([full
        changelog](https://github.com/jenkinsci/remoting/blob/master/CHANGELOG.md))

##### Version 3.14 (September 4, 2018)

-   Swarm client
    -   Update Remoting from 3.21 to 3.26 in order to pick up new stability
        fixes ([full
        changelog](https://github.com/jenkinsci/remoting/blob/master/CHANGELOG.md))
-   Swarm plugin
    -   Update Swarm client to 3.26

##### Version 3.13 (June 8, 2018)

-   Swarm plugin
    -   Update minimal Jenkins Core requirement to 2.60.1
-   Swarm client
    -   Update Remoting to 3.21 to pick up logging and `no_proxy` handling
        fixes ([full
        changelog](https://github.com/jenkinsci/remoting/blob/master/CHANGELOG.md#321))

##### Version 3.12 (March 22, 2018)

-   Swarm client
    -   [JENKINS-50237](https://issues.jenkins-ci.org/browse/JENKINS-50237)
        Update Remoting from 3.18 to 3.19 to pick up the exception
        propagation fix ([full
        changelog](https://github.com/jenkinsci/remoting/blob/master/CHANGELOG.md#319))

##### Version 3.11 (March 19, 2018)

-   Swarm client
    -   [JENKINS-50252](https://issues.jenkins-ci.org/browse/JENKINS-50252)
        Update Remoting from 3.16 to 3.18 to pick up bug fixes and
        serialization diagnosability improvements ([full
        changelog](https://github.com/jenkinsci/remoting/blob/master/CHANGELOG.md))
    -   [\#68](https://github.com/jenkinsci/swarm-plugin/pull/68)
        The plugin now trims input strings for password files specified
        in `-passwordFile`

##### Version 3.10 (February 21, 2018)

-   Swarm plugin
    -   [\#62](https://github.com/jenkinsci/swarm-plugin/pull/62)
        Add ability to download the client directory from the plugin
        installed in Jenkins via `${JENKINS_URL}/swarm/swarm-client.jar`

##### Version 3.9 (February 7, 2018)

-   Swarm plugin
    -   [JENKINS-49292](https://issues.jenkins-ci.org/browse/JENKINS-49292)
        Reduce log level from ALL to INFO in sample logging.properties
        to reduce log spam
-   Swarm client
    -   [\#66](https://github.com/jenkinsci/swarm-plugin/pull/66)
        Add support of the `–passwordFile` option

##### Version 3.8 (January 10, 2018)

-   Swarm client
    -   [\#65](https://github.com/jenkinsci/swarm-plugin/pull/65) Update
        Remoting from 3.15 to 3.16 ([full
        changelog](https://github.com/jenkinsci/remoting/blob/master/CHANGELOG.md))

##### Version 3.7 (December 22, 2017)

-   Swarm client
    -   [\#63](https://github.com/jenkinsci/swarm-plugin/pull/63)
        Require Java 8 (client-side only)
    -   [\#63](https://github.com/jenkinsci/swarm-plugin/pull/63) Update
        Remoting from 3.10.2 to 3.15 ([full
        changelog](https://github.com/jenkinsci/remoting/blob/master/CHANGELOG.md))
    -   [\#61](https://github.com/jenkinsci/swarm-plugin/pull/61)
        Prevent the infinite reconnect cycle in Remoting Launcher, use
        the client's failover logic instead

##### Version 3.6 (October 18, 2017)

-   Update Remoting in Swarm client from 3.4.1 to 3.10.2 ([full
    changelog](https://github.com/jenkinsci/remoting/blob/master/CHANGELOG.md))
-   [\#55](https://github.com/jenkinsci/swarm-plugin/pull/55)
    Introduce the `-pidFile` option, which creates a file with the
    process PID
    -   Errata: The current implementation may cause file descriptor
        leaks in edge cases
-   [JENKINS-43674](https://issues.jenkins-ci.org/browse/JENKINS-43674)
    Prevent `NullPointerException` in Swarm client in HTTPS mode without
    `-disableSslVerification` or `-sslFingerprints`
-   [JENKINS-42098](https://issues.jenkins-ci.org/browse/JENKINS-42098)
    Prevent `LinkageError` when building a Maven project on a Swarm node
    with new Maven versions

##### Version 3.5 (October 11, 2017)

-   [SECURITY-597](https://jenkins.io/security/advisory/2017-10-11/#swarm-plugin-client-bundled-vulnerable-version-of-the-commons-httpclient-library)
    Swarm client bundled version of the commons-httpclient
    library, which was vulnerable to MitM

##### Version 3.4 (April 10, 2017)

-   Add option `-sslFingerprints` providing a possibility to add custom
    SSL trust anchors without adding them to the system store

##### Version 3.3 (February 10, 2017)

-   Finally a release!
-   Add `-logFile` and `-labelsFile` options. Now supports dynamic labels
-   Add support for very large numbers of dynamic labels when using
    `-labelsFile`
-   Remove consecutive slashes in plugin URLs
-   Docker Compose configuration updates
-   Add retry backoff strategy
-   Bump Remoting library to same as Jenkins LTS at the moment
-   Updates to make build and testing pass with new Jenkins plugin
    parent POM work

##### Version 3.2 (February 8, 2017)

-   Failed to release due to INFRA-588

##### Version 3.1 (February 8, 2017)

-   Failed to release due to INFRA-588

##### Version 3.0 (December 27, 2016)

-   Failed to release due to INFRA-588

##### Version 2.3 (November 28, 2016)

-   Failed to release due to INFRA-588

##### Version 2.2 (July 26, 2016)

-   Failed to release due to INFRA-588

##### Version 2.1 (May 20, 2016)

-   Implement [JENKINS-28917](https://issues.jenkins-ci.org/browse/JENKINS-28917) Update
    remoting to one supported by latest LTS
-   `MESOS_TASK_ID` used as Jenkins slave ID if available as environment
    variable (for Mesos/Marathon integration)
-   Updating Jenkins remoting dependency. Swarm client now matches the
    Remoting version in Jenkins 1.625.3 LTS.
-   Implement
    [JENKINS-34593](https://issues.jenkins-ci.org/browse/JENKINS-34593)
    add an option to delete existing clients
-   Add integration test environment based upon Docker compose

##### Version 2.0 (August 3, 2015)

-   Implement [JENKINS-28148](https://issues.jenkins-ci.org/browse/JENKINS-29232) Whitespace
    in tool locations, (breaking change, see
    [\#28](https://github.com/jenkinsci/swarm-plugin/pull/28))
-   Add ability to disable unique ID for clients
    ([\#33](https://github.com/jenkinsci/swarm-plugin/pull/33))
-   Remove unused code and reformat source files

##### Version 1.26 (July 21, 2015)

-   Re-release of 1.25, some artifacts was not properly deployed

##### Version 1.25 (July 21, 2015)

-   Correct
    [JENKINS-29232](https://issues.jenkins-ci.org/browse/JENKINS-29232)
    Set the HTTP Connection:close header to ensure the underlying
    socket is closed
    ([\#29](https://github.com/jenkinsci/swarm-plugin/pull/29))
-   Add a Markdown formatted README to better describe the project for
    GitHub viewers
-   Improve end user reporting of hostname lookup errors
    ([\#30](https://github.com/jenkinsci/swarm-plugin/pull/30))
-   Made Javadoc compile with JDK 8

##### Version 1.24 (April 28, 2015)

-   Correct [JENKINS-26558](https://issues.jenkins-ci.org/browse/JENKINS-26558)
    Clients should provide a unique ID to be used for name collision
    avoidance
    ([\#26](https://github.com/jenkinsci/swarm-plugin/pull/26))
-   Improve printout when Jenkins master is not configured with a URL
    ([\#27](https://github.com/jenkinsci/swarm-plugin/pull/27))

##### Version 1.23 (April 27, 2015)

-   Add the tunnel option to pass it to the Jenkins engine
    ([\#22](https://github.com/jenkinsci/swarm-plugin/pull/22))
-   Minor enhancements to make the Swarm client usable for mere
    detection of Jenkins instances
    ([\#23](https://github.com/jenkinsci/swarm-plugin/pull/22))
-   Correct [JENKINS-24149](https://issues.jenkins-ci.org/browse/JENKINS-24149)
    `LogConfigurationException`
    ([\#24](https://github.com/jenkinsci/swarm-plugin/pull/24))
-   `Computer.toNode()` can return `null`
    ([\#25](https://github.com/jenkinsci/swarm-plugin/pull/25))

##### Version 1.22 (November 28, 2014)

-   Add new option `passwordEnvVariable`
    ([\#21](https://github.com/jenkinsci/swarm-plugin/pull/21))

##### Version 1.21 (November 6, 2014)

-   Instead of constructing the tool location key, just use the existing
    descriptor ([JENKINS-25064](https://issues.jenkins-ci.org/browse/JENKINS-25064),
    see [\#20](https://github.com/jenkinsci/swarm-plugin/pull/20))
-   Use latest Jenkins LTS Remoting library (1.580.1 Jenkins LTS
    version)

##### Version 1.20 (October 8, 2014)

-   Fix up handling of tool locations on Windows
    ([JENKINS-25002](https://issues.jenkins-ci.org/browse/JENKINS-25002),
    see [\#19](https://github.com/jenkinsci/swarm-plugin/pull/19))

##### Version 1.19 (October 6, 2014)

-   Correct bug introduced by 1.18 where the client did not work
    _unless_ you set tool locations
    ([JENKINS-24995](https://issues.jenkins-ci.org/browse/JENKINS-24995),
    see [\#18](https://github.com/jenkinsci/swarm-plugin/pull/18))

##### Version 1.18 (October 2, 2014)

-   Set tool locations from Swarm client,
    ([JENKINS-7543](https://issues.jenkins-ci.org/browse/JENKINS-7543),
    see [\#17](https://github.com/jenkinsci/swarm-plugin/pull/17))

##### Version 1.17 (September 30, 2014)

-   Add `-noRetryAfterConnected` and `-retry` options. These provide
    optional exit strategies for the default unlimited retry loop
-   Require a well-formed master URL, ensuring trailing slash
-   [JENKINS-21892](https://issues.jenkins-ci.org/browse/JENKINS-21892)
    Update Swarm client to send CSRF token
-   Use latest releases of `commons-codec`, `args4j`, and Remoting

##### Version 1.16 (July 1, 2014)

-   Bump remoting to match Jenkins LTS
    ([JENKINS-22730](https://issues.jenkins-ci.org/browse/JENKINS-22730),
    see [\#14](https://github.com/jenkinsci/swarm-plugin/pull/14))

##### Version 1.15

-   *undocumented, or maybe a typo of 1.12?*

##### Version 1.12, 1.11 (January 15, 2014)

-   Use compatible version of `commons-codec`
    ([JENKINS-21155](https://issues.jenkins-ci.org/browse/JENKINS-21155),
    see [\#7](https://github.com/jenkinsci/swarm-plugin/pull/7)
    and [\#8](https://github.com/jenkinsci/swarm-plugin/pull/8))

##### Version 1.10 (October 21, 2013)

-   Swarm 1.9 can't connect to current LTS as `slave.jar` too old
    ([JENKINS-20138](https://issues.jenkins-ci.org/browse/JENKINS-20138))

##### Version 1.9 (May 18), 2013)

-   Add option for specifying `Node.Mode`
    ([\#3](https://github.com/jenkinsci/swarm-plugin/pull/3))

##### Version 1.8 (November 21, 2012)

-   Changing broadcast to send a UDP packet payload of 128 bytes instead
    of 0
-   Allow slave connection without requiring UDP
-   Add `disableSslVerification` option

##### Version 1.6 (March 18, 2012)

-   Fix references from Hudson to Jenkins
-   Swarm client fails to connect to Jenkins when authentication is
    enabled but Authorization is disabled
    ([JENKINS-11663](https://issues.jenkins-ci.org/browse/JENKINS-11663))
-   Support remoting 2.12

##### Version 1.5 (August 11, 2011)

-   Check whether user has `SlaveComputer.CREATE` permission
-   Allow authentication in Swarm plugin
    ([JENKINS-5504](https://issues.jenkins-ci.org/browse/JENKINS-5504))

##### Version 1.4 (August 14, 2010)

-   Fix broken help links
-   Node properties save correctly
-   Add Japanese localization

##### Version 1.3 (January 14, 2010)

-   Fix a packaging problem in the client JAR
    ([JENKINS-5275](https://issues.jenkins-ci.org/browse/JENKINS-5275))

##### Version 1.2 (December 30, 2009)

-   Minor text correction

##### Version 1.1 (July 15, 2009)

-   Add the `-master` option

##### Version 1.0 (May 23, 2009)

-   Initial release
