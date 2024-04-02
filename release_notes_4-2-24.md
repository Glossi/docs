update(general): v2 ux improvements [PRO-130]:

File: package-lock.json:
++ Add `@radix-ui/react-radio-group`

File: package.json:
++ Add `@radix-ui/react-radio-group`


FIle: src/components/IntentSelection.js:
~~ Now works when touched on mobile
~~ Now adjusts size for smaller screen sizes

File: src/components/atoms/PaginationComponent.js:
~~ Infers start point from props

File: src/components/atoms/Tooltip.js:
~~ Added props for more control

File: src/components/atoms/buttons/Button.js:
~~ Improve `onTouchEnd` mobile support

File: src/components/atoms/modals/BrowserDetectModal.js:
-- Styled to match Figma with the addition of a link
![CleanShot 2024-03-28 at 23 22 39](https://github.com/Glossi/glossi-web/assets/19928793/77945550-5d7b-467f-82be-22adaa9014c5)


File: src/components/atoms/modals/ModalComponent.js:
~~ `Escape` no longer closes modals that do not have the `toggle` prop
~~ Improved support for closing by touching outside of the modal

File: src/components/atoms/modals/UploadModelModal.js:
~~ Now opens file dialog on Safari and Firefox

File: src/components/icons/SvgScreens.js:
++ New SVG for `BrowserDetectModal`

File: src/onboarding/OnboardingIntent.js:
~~ Improved repsonsiveness

File: src/onboarding/OnboardingStepper.j
~~ Improved repsonsiveness

File: src/pages/LibraryPage/index.js:
~~ Remembers which page user was on unless they navigate to `/studio` or `/projects`
![CleanShot 2024-03-28 at 23 24 16](https://github.com/Glossi/glossi-web/assets/19928793/593e2b4c-2bd1-4de5-9528-461232580eec)


File: src/pages/ProjectsPage/index.js:
++ Resets pagination on `/library` page when when you visit `/projects` or `/studio`

File: src/studio/StudioMain.js:
++ Resets pagination on `/library` page when when you visit `/projects` or `/studio`

File: src/studio/atoms/AdvancedSettingsDropdown.js:
~~ Added separator
++ Added tooltip prop to `RenderSettingListObject`

File: src/studio/atoms/BackdropGridItem.js:
~~ Improved mobile touch support

File: src/studio/atoms/ModelCardSelect.js:
~~ Improved mobile touch support

File: src/studio/atoms/PaginationSelectionGrid.js:
~~ Improved mobile touch support

File: src/studio/atoms/RadioGroup.js:
++ New component for advanced export settings radio items
![CleanShot 2024-03-28 at 23 25 54](https://github.com/Glossi/glossi-web/assets/19928793/cfeab7f3-7ee7-43a3-abf1-1a4adc0ded7b)


File: src/studio/atoms/RenderSettingListObject.js:
++ Added tooltips to each item
~~ Reworked RadioButtonGroup component
![CleanShot 2024-03-28 at 23 26 50](https://github.com/Glossi/glossi-web/assets/19928793/34bb6609-aff1-49a5-be2d-1a56a3e6559c)


File: src/studio/atoms/SidebarSubHeader.js:
-- Removed color transition on hover
~~ Improved mobile touch events

File: src/studio/layout-grid/header/StudioHeaderLeft.js:
~~ Now possible to exit studio on mobile

File: src/studio/modals/ExportModal.js:
~~ Massages `"Off"` value to `false` for convenience

File:src/studio/modals/RenderActiveModal.js:
~~ Shrank `Preparing` modal
![CleanShot 2024-03-28 at 23 29 28](https://github.com/Glossi/glossi-web/assets/19928793/e7426c17-88d7-4f71-a0e5-f9745a84da96)


File: src/studio/pixel-stream/store.ts:
++ Added `userPaginationState`

File: src/studio/right-sidebars/EditBackdropStyleSidebar.js:
~~ Passing empty value for label name to avoid propTypes error

File: src/studio/right-sidebars/ProjectElementsSidebar.js:
~~ Switch `Change` button to `<Button>` component

File: src/utils/constants.js:
~~ Modify `renderSettings` for advanced settings dropdown
-- Removed `iPad` from the blocked mobile devices list