This is updated fork to - **[A TestListener that integrates with XHProf](https://github.com/phpunit/phpunit-testlistener-xhprof)**

Example XML configuration for activating this listener:
```xml
<listeners>
    <listener class="PHPUnit\XHProfTestListener\XHProfTestListener">
        <arguments>
            <array>
                <element key="xhprofLibFile">
                    <string>/var/www/xhprof_lib/utils/xhprof_lib.php</string>
                </element>
                <element key="xhprofRunsFile">
                    <string>/var/www/xhprof_lib/utils/xhprof_runs.php</string>
                </element>
                <element key="xhprofWeb">
                    <string>http://localhost/xhprof_html/index.php</string>
                </element>
                <element key="appNamespace">
                    <string>Doctrine2</string>
                </element>
                <element key="xhprofFlags">
                    <string>XHPROF_FLAGS_CPU,XHPROF_FLAGS_MEMORY</string>
                </element>
                <element key="xhprofIgnore">
                    <string>call_user_func,call_user_func_array</string>
                </element>
            </array>
        </arguments>
    </listener>
</listeners>
```
