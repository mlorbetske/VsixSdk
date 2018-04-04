**What is this?**

This is an attempt to allow VSIX projects to be able to use "SDK" style projects


**Prerequisites**

Microsoft Visual Studio 2017.6 or higher


**Building the sample**

First, you'll need to pack the SDK package and the "meta" package (in Visual
Studio, you can do this by opening `Microsoft.Vsix.Sdk.sln`, right-clicking
each project and selecting `Pack`).

Now, opening the `samples\Samples.sln` should work & things like F5 should
work as usual.


**Known issues**

Updating the vsixmanifest doesn't necessarily cause things to be fully re-built.
 - Doing a clean & rebuild should get things working again
 
The designer for the vsixmanifest file doesn't work
 - This is a known limitation for now
 
The item templates for extensiblity projects don't show up
 - This is a known limitation for now

**Credit**

A lot of what's here is adapted from [AArnott/VSIXProjectWithPackageReferences](https://github.com/AArnott/VSIXProjectWithPackageReferences/blob/netsdk/VSIXProject11/VSIXProject11.csproj)
