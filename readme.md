# AuraGem Opensource Copyleft License

The AuraGem Opensource Copyleft License (AOCL) addresses modern software development needs while preserving open source freedoms. This license is designed for developers who want their code to remain open while enabling practical business use.

Software freedom includes the rights to use, copy, modify, rebuild, and distribute software. These rights must remain protected regardless of how software is delivered or deployed. When software is distributed over networks or integrated into larger systems, these fundamental freedoms should not be diminished.

AOCL provides these protections through:
- Clear distinctions between Derivative and Dependent works
- Explicit protections for irrevocable redistribution and rebuilding rights
- Modern provisions for network-based software delivery
- Strong patent protections and attribution requirements
- Fixed versioning to ensure consistent interpretation

This license strikes a balance between protecting user freedoms and enabling practical integration. It is more protective than permissive licenses while being more pragmatic than traditional strong copyleft licenses.

Recent events have highlighted how traditional open source licenses could be manipulated through creative interpretation to restrict redistribution and rebuilding rights - a practice intended to discriminate against particular persons, groups, and fields of endeavor. It represents a real threat to open source principles that risks reverting the ecosystem to an era without open source freedoms. AOCL explicitly closes potential loopholes preventing any attempt to terminate, discourage, impede, or restrict rights granted by this license when users exercise their open source freedoms. Simply redistributing and rebuilding code is part of the terms and spirit of open source, whether or not it adds value or modifies the code. While commercial entities that have built their businesses on the backs of the open source community may find this inconvenient for their "enterprise" business models, when software is open source, it should follow the terms of open source without impedement.

## Details

### Permissions
* Commercial Use
* Distribution
* Modification
* Patent Use
* Private Use

### Conditions
* Disclose Source
* License and copyright notice
* Same license (library; Derivative Works only)
* Network use is distribution (attribution for Dependent Works, copyleft for Derivative Works)
* State changes

### Limitations
* Warranty
* Liability
* Trademark Use

## Compatibility with Other Licenses

### Permissive License Compatibility

1. MIT License - Two-way Compatibility
   * MIT code can be included in AOCL projects
   * AOCL code can be used in MIT projects if:
     - Attribution requirements are met
     - Network service provisions are followed
     - The MIT project qualifies as a Dependent Work

2. BSD Licenses (2-clause, 3-clause) - Two-way Compatibility
   * Similar to MIT compatibility
   * Must maintain BSD attribution notices
   * Compatible with AOCL's attribution requirements

3. Mozilla Public License 2.0 - Two-way Compatibility with file separation
   * File-level copyleft aligns with AOCL's dependent work provisions
   * Can be used together in the same project
   * Each file retains its original license

## Determining Derivative vs. Dependent Works

### Overview

Using the Software as a library via package/module import, inclusion, process spawning, and static or dynamic linking, qualifies as a Dependent Work as long as there's no modifications to the Software. They are subject only to the Attribution, Trademark, Warranty, and Liability Limitations and Conditions.

Modification and new code added to the Software such that the Software cannot compile without it (aka. Additions) qualify as Derivative Works. They are subject to *all* of the Conditions and Limitations of the AOCL License.

> 1.5 "Derivative Work" means any work that, given the definitions in Section 1.4:
>    a) Contains, is based on, or is derived from the Software through Modification, Enhancement, or Addition; or
>    b) Incorporates any part of the Software's source code with modifications; or
>    c) Would require permission under copyright law from the Original Authors or Copyright Holders due to modification or adaptation of the Software.
>
> 1.6 "Dependent Work" means any work that, diven the definitions in Section 1.4:
>    a) Uses or Interacts with the Software without modification; or
>    b) Incorporates the the unmodified Software through compilation, linking, or other standard integration methods; or
>    c) Relies on the Software's functionality through well-defined interfaces without modifying the Software itself.
>
>    Such Dependent Works are subject to Sections 4 (Attribution), 5 (Trademark Usage), and 8 (Network Usage) of this license, while retaining their independence in other aspects.

### Decision Tree

To determine whether your work is a Derivative Work or a Dependent Work, follow this decision tree:

1. Does your work modify the Software's Source Code?
   - Yes: It is a Derivative Work.
   - No: Proceed to question 2.

2. Does your work create a technical dependency on the Software (e.g., requiring additional code to compile or function)?
   - Yes: It is a Derivative Work.
   - No: Proceed to question 3.

3. Does your work integrate the Software's Source Code in a way that makes the integrated parts interdependent with your work?
   - Yes: It is a Derivative Work.
   - No: Proceed to question 4.

4. Does your work use the Software as is, without modification, and interact with it solely through standard protocols, operating system interfaces, or linking?
   - Yes: It is a Dependent Work.
   - No: Consult the full definitions in Section 1.4 for further clarification.

Examples of Common Integration Patterns:
- Importing a library and calling its functions: Dependent work
- Copying and modifying library code: Derivative work
- Using library through API calls: Dependent work
- Extending library classes/interfaces: Derivative work
