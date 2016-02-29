Nutch Initial Scoring Filter (scoring-initial)
======================

Scoring Filter plugin for Nutch 2.3.
Initial static boost for all page crawling site

Usage
======================

```xml
<property>
    <name>initial.static.score</name>
    <value>3.0</value>
    <description>
        Initial boost value for all crawled page.
    </description>
</property>
```

```xml
<property>
    <name>plugin.includes</name>
    <value>protocol-http|urlfilter-regex|parse-(html|tika)|external-filter|index-(basic|anchor)|urlnormalizer-(pass|regex|basic)|scoring-initial</value>
    <description>
        Regular expression naming plugin directory names to
        include.  Any plugin not matching this expression is excluded.
        In any case you need at least include the nutch-extensionpoints plugin. By
        default Nutch includes crawling just HTML and plain text via HTTP,
        and basic indexing and search plugins. In order to use HTTPS please enable 
        protocol-httpclient, but be aware of possible intermittent problems with the 
        underlying commons-httpclient library.
    </description>
</property>
```

