Bridge between `l10n_pe_hr_payroll` and `one2many_search_widget`: adds the search box to the
payslip "Other Inputs" and "Salary Computation" lists.

It lives here, and not in `l10n_pe_hr_payroll`, because the widget is AGPL-3 and the payroll
module is OPL-1. It installs itself (`auto_install`) when both modules are installed; on a
database that already has both, install it once from Apps (a module update does not trigger
`auto_install`).
