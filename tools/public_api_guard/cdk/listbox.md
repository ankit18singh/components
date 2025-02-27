## API Report File for "components-srcs"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { ActiveDescendantKeyManager } from '@angular/cdk/a11y';
import { AfterContentInit } from '@angular/core';
import { BooleanInput } from '@angular/cdk/coercion';
import { ChangeDetectorRef } from '@angular/core';
import { ControlValueAccessor } from '@angular/forms';
import { Highlightable } from '@angular/cdk/a11y';
import * as i0 from '@angular/core';
import { ListKeyManagerOption } from '@angular/cdk/a11y';
import { OnDestroy } from '@angular/core';
import { QueryList } from '@angular/core';
import { SelectionModel } from '@angular/cdk/collections';
import { Subject } from 'rxjs';

// @public (undocumented)
export class CdkListbox<T = unknown> implements AfterContentInit, OnDestroy, ControlValueAccessor {
    protected readonly changeDetectorRef: ChangeDetectorRef;
    get compareWith(): undefined | ((o1: T, o2: T) => boolean);
    set compareWith(fn: undefined | ((o1: T, o2: T) => boolean));
    deselect(option: CdkOption<T>): void;
    deselectValue(value: T): void;
    protected readonly destroyed: Subject<void>;
    get disabled(): boolean;
    set disabled(value: BooleanInput);
    protected readonly element: HTMLElement;
    get enabledTabIndex(): number | null;
    set enabledTabIndex(value: number | null);
    focus(): void;
    protected _getAriaActiveDescendant(): string | null | undefined;
    protected _getTabIndex(): number | null;
    protected _handleFocus(): void;
    protected _handleFocusOut(event: FocusEvent): void;
    protected _handleKeydown(event: KeyboardEvent): void;
    get id(): string;
    set id(value: string);
    isSelected(option: CdkOption<T>): boolean;
    isValueSelected(value: T): boolean;
    protected listKeyManager: ActiveDescendantKeyManager<CdkOption<T>>;
    get multiple(): boolean;
    set multiple(value: BooleanInput);
    get navigateDisabledOptions(): BooleanInput;
    set navigateDisabledOptions(skip: BooleanInput);
    get navigationWrapDisabled(): BooleanInput;
    set navigationWrapDisabled(wrap: BooleanInput);
    // (undocumented)
    ngAfterContentInit(): void;
    // (undocumented)
    ngOnDestroy(): void;
    protected options: QueryList<CdkOption<T>>;
    get orientation(): 'horizontal' | 'vertical';
    set orientation(value: 'horizontal' | 'vertical');
    registerOnChange(fn: (value: readonly T[]) => void): void;
    registerOnTouched(fn: () => {}): void;
    select(option: CdkOption<T>): void;
    protected selectionModel: ListboxSelectionModel<T>;
    selectValue(value: T): void;
    _setActiveOption(option: CdkOption<T>): void;
    setAllSelected(isSelected: boolean): void;
    setDisabledState(isDisabled: boolean): void;
    toggle(option: CdkOption<T>): void;
    toggleValue(value: T): void;
    protected triggerOption(option: CdkOption<T> | null): void;
    protected triggerRange(trigger: CdkOption<T> | null, from: number, to: number, on: boolean): void;
    get useActiveDescendant(): boolean;
    set useActiveDescendant(shouldUseActiveDescendant: BooleanInput);
    get value(): readonly T[];
    set value(value: readonly T[]);
    readonly valueChange: Subject<ListboxValueChangeEvent<T>>;
    writeValue(value: readonly T[]): void;
    // (undocumented)
    static ɵdir: i0.ɵɵDirectiveDeclaration<CdkListbox<any>, "[cdkListbox]", ["cdkListbox"], { "id": "id"; "enabledTabIndex": "tabindex"; "value": "cdkListboxValue"; "multiple": "cdkListboxMultiple"; "disabled": "cdkListboxDisabled"; "useActiveDescendant": "cdkListboxUseActiveDescendant"; "orientation": "cdkListboxOrientation"; "compareWith": "cdkListboxCompareWith"; "navigationWrapDisabled": "cdkListboxNavigationWrapDisabled"; "navigateDisabledOptions": "cdkListboxNavigatesDisabledOptions"; }, { "valueChange": "cdkListboxValueChange"; }, ["options"], never, false, never>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<CdkListbox<any>, never>;
}

// @public (undocumented)
export class CdkListboxModule {
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<CdkListboxModule, never>;
    // (undocumented)
    static ɵinj: i0.ɵɵInjectorDeclaration<CdkListboxModule>;
    // (undocumented)
    static ɵmod: i0.ɵɵNgModuleDeclaration<CdkListboxModule, [typeof i1.CdkListbox, typeof i1.CdkOption], never, [typeof i1.CdkListbox, typeof i1.CdkOption]>;
}

// @public
export class CdkOption<T = unknown> implements ListKeyManagerOption, Highlightable, OnDestroy {
    readonly _clicked: Subject<MouseEvent>;
    deselect(): void;
    protected destroyed: Subject<void>;
    get disabled(): boolean;
    set disabled(value: BooleanInput);
    readonly element: HTMLElement;
    get enabledTabIndex(): number | null;
    set enabledTabIndex(value: number | null);
    focus(): void;
    getLabel(): string;
    protected _getTabIndex(): number | null;
    protected _handleFocus(): void;
    get id(): string;
    set id(value: string);
    isActive(): boolean;
    isSelected(): boolean;
    protected readonly listbox: CdkListbox<T>;
    // (undocumented)
    ngOnDestroy(): void;
    select(): void;
    setActiveStyles(): void;
    setInactiveStyles(): void;
    toggle(): void;
    typeaheadLabel: string;
    value: T;
    // (undocumented)
    static ɵdir: i0.ɵɵDirectiveDeclaration<CdkOption<any>, "[cdkOption]", ["cdkOption"], { "id": "id"; "value": "cdkOption"; "typeaheadLabel": "cdkOptionTypeaheadLabel"; "disabled": "cdkOptionDisabled"; "enabledTabIndex": "tabindex"; }, {}, never, never, false, never>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<CdkOption<any>, never>;
}

// @public
export interface ListboxValueChangeEvent<T> {
    readonly listbox: CdkListbox<T>;
    readonly option: CdkOption<T> | null;
    readonly value: readonly T[];
}

// (No @packageDocumentation comment for this package)

```
