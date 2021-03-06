
MonoCompilerAsAService is just the [Mono](http://www.mono-project.com) 2.10 C# compiler as a small project.    
This project is based on [Frank A. Krueger's](http://www.twitter.com/praeclarum) work porting this compiler to [Silverlight](https://github.com/praeclarum/runcs). Try it out at: [runcsharp.com](http://runcsharp.com).

#### Usage

    _Compiler = new Runner();
    Console.WriteLine(_Compiler.Execute("Math.Abs(-42);"));
    Console.WriteLine(_Compiler.Execute("Math.Sin(Math.PI / 6);"));
    Console.WriteLine(_Compiler.Execute("class Fact { public int Run(int n) { return n <= 0 ? 1 : n*Run(n-1); } }"));
    Console.WriteLine(_Compiler.Execute("new Fact().Run(5);"));
    Console.WriteLine(_Compiler.Execute("\"abcdefgh\".Substring(1, 2);"));
    Console.WriteLine(_Compiler.Execute("var str = \"Hello World!\";"));
    Console.WriteLine(_Compiler.Execute("Print (str);"));

	
#### CSharpShell

You can also use a nice interactive CSharpShell based on Mono's read-eval-print loop...

![CSharpShell screenshot](/ahzf/MonoCompilerAsAService/raw/master/doc/CSharpShell_InAction1.png)

	
#### License

Just praise the Mono crew. I did nothing... But anyway [MonoCompilerAsAService](http://github.com/ahzf/MonoCompilerAsAService) is released under the [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0). For details see the [LICENSE](/ahzf/MonoCompilerAsAService/blob/master/LICENSE) file.
To suggest a feature, report a bug or general discussion: [http://github.com/ahzf/MonoCompilerAsAService/issues](http://github.com/ahzf/MonoCompilerAsAService/issues)    
If you want to help or contribute source code to this project, please use the same license.   


#### Acknowledgments

Please read the [NOTICE](/ahzf/MonoCompilerAsAService/blob/master/NOTICE) file for further credits.
