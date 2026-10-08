# Guacamole

This familiar recipe carries the Carpentries Git lesson into the collaboration and conflict portion of the OSU Libraries workshop.

## Ingredients

- 2 ripe avocados
- 1 lime
- 1/4 teaspoon salt
<<<<<<< HEAD
- 1/2 fresh salsa
=======
<<<<<<< HEAD
- 1/2 cup homemade salsa
=======
-1/2 fresh salsa
>>>>>>> 409b2ac5f4b7f8b2b6d95343f7f6c357601ea398
>>>>>>> 6a3a7ceb343f452b66f8854fd3d3bc9449a5835d

## Method

1. Halve and pit the avocados.
2. Scoop the avocado into a bowl.
3. Mash the avocado until smooth.
4. Stir in lime juice, salt, onion, and cilantro.
5. Taste and adjust seasoning.

## Workshop use

The reading list in `build-example/books.md` is the main shared BUILD artifact. This recipe remains available as the familiar Carpentries continuity object for a controlled same-line conflict.

When directed by the instructor, overlapping edits to step 3 can create the conditions for a merge conflict.

Keep the states distinct:

1. another collaborator pushes work;
2. your local clone may have different work;
3. your push can be rejected because the remote has history you do not yet have;
4. you pull/integrate;
5. only if Git cannot reconcile overlapping changes does it report a merge conflict;
6. a human decides the intended content, stages the resolution, commits, and shares it.

Git can preserve competing text. It cannot decide which guacamole tastes better.
