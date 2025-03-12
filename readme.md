# AuraGem Opensource Copyleft License

The AuraGem Opensource Copyleft License (AOCL) is designed to provide a balanced approach to copyleft that ensures modifications to source code remain open while enabling flexible integration through linking interfaces, UIs, standard library usage, and data exchange.

AOCL protects the rights of creators through attribution requirements and patent provisions while addressing modern software delivery methods, including network services (e.g., SaaS).

By distinguishing between Derivative and Dependent works, the license balances copyleft with flexibility. Derivative works are subject to copyleft under the AOCL license. Dependent Works can be licensed independently from the AOCL-licensed Software being depended on. This allows AOCL-licensed Software to be used as a library for static linking, dynamic linking, FFI, or standard inclusion as a library without modification, which is common in programming languages like Rust and Golang.

Unlike other open source licenses, AOCL is a fixed version without automatic version upgrading, removing confusion about which version applies to a given software, whether derivatives can or cannot utilize "later versions" of this license, and ensuring all modifications to software under this license can be upstreamed without additional restrictions placed on those modifications.

This license represents a middle ground that is more protective than permissive licenses and more pragmatic than traditional strong copyleft licenses, allowing the software to be used in widely diverse contexts with appropriate attribution and patent protections, and maintaining a consistent set of obligations that cannot change over time without the explicit permission of the original authors or copyright holders of the software. By choosing this license, you contribute to a collaborative ecosystem that balances freedom, recognition, and practical adoption.

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

## Determining Derivative vs. Dependent Works

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
