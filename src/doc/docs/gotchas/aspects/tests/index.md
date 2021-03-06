!!! question "Can I add an annotation to skip tests the way it normally works with junit?"

    No, it is not supported. You have to comment out the test case. The only statement that supports this behaviour is the 
    assert statement of KernelF ([AssertTestItem](http://127.0.0.1:63320/node?ref=r%3Aba7faab6-2b80-43d5-8b95-0c440665312c%28org.iets3.core.expr.tests.structure%29%2F543569365052056266))

!!! warning "Tests have a long warm up time and run slowly."
    
    When running the tests from a run configuration, enable "Execute in the same process" in the configuration settings.
    Also check the box "Allow parallel run" ([official documentation](https://www.jetbrains.com/help/mps/testing-languages.html#runningthetests)).

!!! warning "Tests are not running at all."

    A [test info node](http://127.0.0.1:63320/node?ref=r%3A00000000-0000-4000-0000-011c89590388%28jetbrains.mps.lang.test.structure%29%2F5097124989038916362) has to
    be added to the model of the tests, so that the tests can find the path of the project. The project path also has to be set
    in this node. Make sure that variables that are used in this path are set in Preferences->Appearance&Behavior->Path Variables.
    ([official documentation](https://www.jetbrains.com/help/mps/testing-languages.html#testinfo))

!!! question "How do I create a TestInfo node for my tests?"
    Specific Languages Blog &mdash; [How to create a TestInfo node for your tests](https://specificlanguages.com/posts/how-to-create-testinfo-node-for-your-tests/){target=_blank}

!!! warning "How do node tests work?"
    Specific Languages Blog &mdash; [How do node tests work?](https://specificlanguages.com/posts/2022-02/23-how-node-tests-work/){target=_blank}