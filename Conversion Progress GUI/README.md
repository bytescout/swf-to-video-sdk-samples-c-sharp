## conversion progress GUI in C# using ByteScout SWF To Video SDK

### Make conversion progress GUI in C#: ### Tutorial on how to do conversion progress GUI in C#

On this page you will learn from code samples for programming in C#. ByteScout SWF To Video SDK helps with conversion progress GUI in C#. ByteScout SWF To Video SDK is the specialized software development kit for programmers who need to add SWF (Flash Macromedia) to video conversion into their app. Supports WMV and AVI video output with sound as can take input flash movies with variables, actionscripts, dynamic files as input. You can control output video size, framerate, video and audio quality.

C#, code samples for C#, developers help to speed up the application development and writing a code when using ByteScout SWF To Video SDK. Follow the instruction from the scratch to work and copy and paste code for C# into your editor. Code testing will allow the function to be tested and work properly with your data.

ByteScout SWF To Video SDK free trial version is available for download from our website. Free trial also includes programming tutorials along with source code samples.

## REQUEST FREE TECH SUPPORT

[Click here to get in touch](https://bytescout.zendesk.com/hc/en-us/requests/new?subject=ByteScout%20SWF%20To%20Video%20SDK%20Question)

or just send email to [support@bytescout.com](mailto:support@bytescout.com?subject=ByteScout%20SWF%20To%20Video%20SDK%20Question) 

## ON-PREMISE OFFLINE SDK 

[Get Your 60 Day Free Trial](https://bytescout.com/download/web-installer?utm_source=github-readme)
[Explore SDK Docs](https://bytescout.com/documentation/index.html?utm_source=github-readme)
[Sign Up For Online Training](https://academy.bytescout.com/)


## ON-DEMAND REST WEB API

[Get your API key](https://pdf.co/documentation/api?utm_source=github-readme)
[Explore Web API Documentation](https://pdf.co/documentation/api?utm_source=github-readme)
[Explore Web API Samples](https://github.com/bytescout/ByteScout-SDK-SourceCode/tree/master/PDF.co%20Web%20API)

## VIDEO REVIEW

[https://www.youtube.com/watch?v=NEwNs2b9YN8](https://www.youtube.com/watch?v=NEwNs2b9YN8)




<!-- code block begin -->

##### ****ConversionProgressGUI.VS2005.csproj:**
    
```
<Project DefaultTargets="Build" xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
  <PropertyGroup>
    <Configuration Condition=" '$(Configuration)' == '' ">Debug</Configuration>
    <Platform Condition=" '$(Platform)' == '' ">AnyCPU</Platform>
    <ProductVersion>8.0.50727</ProductVersion>
    <SchemaVersion>2.0</SchemaVersion>
    <ProjectGuid>{525EDC14-A580-4410-8A81-5ECB9B4B3F63}</ProjectGuid>
    <OutputType>WinExe</OutputType>
    <AppDesignerFolder>Properties</AppDesignerFolder>
    <RootNamespace>ConversionProgressGUI</RootNamespace>
    <AssemblyName>ConversionProgressGUI</AssemblyName>
  </PropertyGroup>
  <PropertyGroup Condition=" '$(Configuration)|$(Platform)' == 'Debug|x86' ">
    <DebugSymbols>true</DebugSymbols>
    <OutputPath>bin\x86\Debug\</OutputPath>
    <DefineConstants>DEBUG;TRACE</DefineConstants>
    <DebugType>full</DebugType>
    <PlatformTarget>x86</PlatformTarget>
    <ErrorReport>prompt</ErrorReport>
  </PropertyGroup>
  <PropertyGroup Condition=" '$(Configuration)|$(Platform)' == 'Release|x86' ">
    <OutputPath>bin\x86\Release\</OutputPath>
    <DefineConstants>TRACE</DefineConstants>
    <Optimize>true</Optimize>
    <DebugType>pdbonly</DebugType>
    <PlatformTarget>x86</PlatformTarget>
    <ErrorReport>prompt</ErrorReport>
  </PropertyGroup>
  <ItemGroup>
    <Reference Include="System" />
    <Reference Include="System.Data" />
    <Reference Include="System.Deployment" />
    <Reference Include="System.Drawing" />
    <Reference Include="System.Windows.Forms" />
    <Reference Include="System.Xml" />
  </ItemGroup>
  <ItemGroup>
  </ItemGroup>
  <ItemGroup>
    <Compile Include="Form1.cs">
      <SubType>Form</SubType>
    </Compile>
    <Compile Include="Form1.Designer.cs">
      <DependentUpon>Form1.cs</DependentUpon>
    </Compile>
    <Compile Include="Program.cs" />
    <Compile Include="Properties\AssemblyInfo.cs" />
    <EmbeddedResource Include="Form1.resx">
      <SubType>Designer</SubType>
      <DependentUpon>Form1.cs</DependentUpon>
    </EmbeddedResource>
    <EmbeddedResource Include="Properties\Resources.resx">
      <Generator>ResXFileCodeGenerator</Generator>
      <LastGenOutput>Resources.Designer.cs</LastGenOutput>
      <SubType>Designer</SubType>
    </EmbeddedResource>
    <Compile Include="Properties\Resources.Designer.cs">
      <AutoGen>True</AutoGen>
      <DependentUpon>Resources.resx</DependentUpon>
      <DesignTime>True</DesignTime>
    </Compile>
    <None Include="Properties\Settings.settings">
      <Generator>SettingsSingleFileGenerator</Generator>
      <LastGenOutput>Settings.Designer.cs</LastGenOutput>
    </None>
    <Compile Include="Properties\Settings.Designer.cs">
      <AutoGen>True</AutoGen>
      <DependentUpon>Settings.settings</DependentUpon>
      <DesignTimeSharedInput>True</DesignTimeSharedInput>
    </Compile>
  </ItemGroup>
  <ItemGroup>
    <COMReference Include="BytescoutSWFToVideo">
      <Guid>{E76CD51E-7817-4D3E-8DD6-A71518D5AEC7}</Guid>
      <VersionMajor>1</VersionMajor>
      <VersionMinor>0</VersionMinor>
      <Lcid>0</Lcid>
      <WrapperTool>tlbimp</WrapperTool>
      <Isolated>False</Isolated>
    </COMReference>
    <COMReference Include="stdole">
      <Guid>{00020430-0000-0000-C000-000000000046}</Guid>
      <VersionMajor>2</VersionMajor>
      <VersionMinor>0</VersionMinor>
      <Lcid>0</Lcid>
      <WrapperTool>primary</WrapperTool>
      <Isolated>False</Isolated>
    </COMReference>
  </ItemGroup>
  <ItemGroup>
    <Content Include="test.swf">
      <CopyToOutputDirectory>Always</CopyToOutputDirectory>
    </Content>
  </ItemGroup>
  <Import Project="$(MSBuildBinPath)\Microsoft.CSharp.targets" />
  <!-- To modify your build process, add your task inside one of the targets below and uncomment it. 
       Other similar extension points exist, see Microsoft.Common.targets.
  <Target Name="BeforeBuild">
  </Target>
  <Target Name="AfterBuild">
  </Target>
  -->
</Project>
```

<!-- code block end -->    

<!-- code block begin -->

##### ****Form1.Designer.cs:**
    
```
namespace ConversionProgressGUI
{
    partial class Form1
    {
        /// <summary>
        /// Required designer variable.
        /// </summary>
        private System.ComponentModel.IContainer components = null;

        /// <summary>
        /// Clean up any resources being used.
        /// </summary>
        /// <param name="disposing">true if managed resources should be disposed; otherwise, false.</param>
        protected override void Dispose(bool disposing)
        {
            if (disposing && (components != null))
            {
                components.Dispose();
            }
            base.Dispose(disposing);
        }

        #region Windows Form Designer generated code

        /// <summary>
        /// Required method for Designer support - do not modify
        /// the contents of this method with the code editor.
        /// </summary>
        private void InitializeComponent()
        {
			this.buttonConvert = new System.Windows.Forms.Button();
			this.label1 = new System.Windows.Forms.Label();
			this.progressBar1 = new System.Windows.Forms.ProgressBar();
			this.SuspendLayout();
			// 
			// buttonConvert
			// 
			this.buttonConvert.Location = new System.Drawing.Point(18, 67);
			this.buttonConvert.Name = "buttonConvert";
			this.buttonConvert.Size = new System.Drawing.Size(254, 23);
			this.buttonConvert.TabIndex = 0;
			this.buttonConvert.Text = "Convert test.swf with conversion preview";
			this.buttonConvert.UseVisualStyleBackColor = true;
			this.buttonConvert.Click += new System.EventHandler(this.buttonConvert_Click);
			// 
			// label1
			// 
			this.label1.AutoSize = true;
			this.label1.Font = new System.Drawing.Font("Microsoft Sans Serif", 8.25F, System.Drawing.FontStyle.Bold, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
			this.label1.Location = new System.Drawing.Point(15, 9);
			this.label1.Name = "label1";
			this.label1.Size = new System.Drawing.Size(126, 13);
			this.label1.TabIndex = 2;
			this.label1.Text = "Conversion progress:";
			// 
			// progressBar1
			// 
			this.progressBar1.Location = new System.Drawing.Point(18, 28);
			this.progressBar1.Name = "progressBar1";
			this.progressBar1.Size = new System.Drawing.Size(254, 23);
			this.progressBar1.TabIndex = 3;
			// 
			// Form1
			// 
			this.AutoScaleDimensions = new System.Drawing.SizeF(6F, 13F);
			this.AutoScaleMode = System.Windows.Forms.AutoScaleMode.Font;
			this.ClientSize = new System.Drawing.Size(284, 102);
			this.Controls.Add(this.progressBar1);
			this.Controls.Add(this.label1);
			this.Controls.Add(this.buttonConvert);
			this.Name = "Form1";
			this.StartPosition = System.Windows.Forms.FormStartPosition.CenterScreen;
			this.Text = "Form1";
			this.ResumeLayout(false);
			this.PerformLayout();

        }

        #endregion

		private System.Windows.Forms.Button buttonConvert;
        private System.Windows.Forms.Label label1;
		private System.Windows.Forms.ProgressBar progressBar1;
    }
}


```

<!-- code block end -->    

<!-- code block begin -->

##### ****Form1.cs:**
    
```
using System;
using System.Windows.Forms;

using BytescoutSWFToVideo;

namespace ConversionProgressGUI
{
    public partial class Form1 : Form
    {
		public const int WM_APP = 0x8000;
		public const int WM_CONVERSION_PROGRESS = WM_APP + 1; 

        SWFToVideoClass swf = new SWFToVideoClass();

        public Form1()
        {
            InitializeComponent();
        }

        private void buttonConvert_Click(object sender, EventArgs e)
        {
            if (!swf.IsRunning)
            {
                swf.SWFConversionMode = SWFConversionModeType.SWFAnimation;
                swf.ConversionTimeOut = 5000;

                swf.InputSWFFileName = "test.swf";
                swf.OutputVideoFileName = "test.wmv";

				swf.SetProgressNotifyWindow(Handle.ToInt32(), WM_CONVERSION_PROGRESS, 0);

                swf.Run();
            }
        }

		protected override void WndProc(ref Message m)
		{
			if (m.HWnd == Handle && m.Msg == WM_CONVERSION_PROGRESS)
			{
				progressBar1.Value = m.WParam.ToInt32();
			}

			base.WndProc(ref m);
		} 
    }
}

```

<!-- code block end -->    

<!-- code block begin -->

##### ****Program.cs:**
    
```
// x64 IMPORTANT NOTE: set CPU to x86 to build in x86 mode. WHY? Because flash is not supported on x64 platform currently at all
using System;
using System.Windows.Forms;

namespace ConversionProgressGUI
{
    static class Program
    {
        /// <summary>
        /// The main entry point for the application.
        /// </summary>
        [STAThread]
        static void Main()
        {
            Application.EnableVisualStyles();
            Application.SetCompatibleTextRenderingDefault(false);
            Application.Run(new Form1());
        }
    }
}

```

<!-- code block end -->