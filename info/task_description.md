> A crystal or crystalline solid is a solid material whose constituents, such as atoms, molecules or ions, are
> arranged in a highly ordered microscopic structure, forming a crystal lattice that extends in all directions.
> The scientific definition of a "crystal" is based on the microscopic arrangement of atoms inside it,
> called the crystal structure. A crystal is a solid where the atoms form a periodic arrangement.

Because crystals are such an important resource, systems must be put in place to check the crystal quality during
the growth and harvest periods. For our initial tests, we use random spot checks on the atomic lines composing each
of the crystals. This crystal type contains two atoms composing the elements "X" (Xenatom) and "Z" (Zorium). In a
well grown crystal, these atoms should alternate down the atomic line.

You are given a random line from crystal lattice as a sequence of letters "X" and "Z". The good line should have the
periodic arrangement (one by one) as ["X", "Z", "X", "Z"]. If any atoms are repeated, then this crystal is broken.

![Rows](https://checkio.s3.amazonaws.com/task/media/645f698652904dc3ba29931333aad060/rows.svg)

**Input:** Atomic lines as a list of strings.

**Output:** The crystal quality as a boolean.


**Example:**

```python
check_line(["X", "Z", "X"]) == True
check_line(["X", "Z", "X", "X"]) == False
```

**How it is used:**

This is first simple data structure and here you can learn how to work with a list. It's a simple concept which you
can solve by just pausing to think.

**Precondition:**
```python
1 < len(line) <= 1000
all(ch in "XZ" for ch in line)
```